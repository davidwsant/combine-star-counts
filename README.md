### Welcome to combine_star_counts.py
usage: ./combine_star_counts.py [-h] [-c COUNT_FILES [COUNT_FILES ...]] [-o OUTPUT_PREFIX]

This program has been designed to combine the counts generated by the RNA-seq aligner, STAR.
By default, three files will be output: one containing unstranded read counts, one containing
first-read counts, and one containing second-read counts.
```
Example usage: ./combine_star_counts.py -c *ReadsPerGene.out.tab -o Human
```

optional arguments:

  -h, --help            show this help message and exit

  -c COUNT_FILES [COUNT_FILES ...], --count_files COUNT_FILES [COUNT_FILES ...]

                        This is an optional way to use the command line to list the ReadsPerGene.out.tab
                        files generated by STAR. These files typically end in 'ReadsPerGene.out.tab'. If
                        you do use this option to specify the count files, all files ending in
                        'ReadsPerGene.out.tab' in your current working directory will be used.

  -o OUTPUT_PREFIX, --output_prefix OUTPUT_PREFIX

                        This is the prefix that will be used for the output files. Default is 'Combined'
