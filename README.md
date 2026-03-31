# wf-singlecell-seekone
The software was developed by Yong Mao (Wuhan Benagen Tech Solutions Company Limited) based on the wf-singlecell v3.3.4 (https://github.com/epi2me-labs/wf-single-cell). It extends support for the SeekOne® single-cell platform in combination with nanopore long-read sequencing. Notably, the original functionality for 10x single-cell and Visium HD full-length data has been retained. The software is publicly available to all researchers.

Brief Manual
To run wf-singlecell-seekoneV1 successfully, nextflow and other dependent tools need be installed.

The detailed manual information can achieved by the command : nextflow run wf-single-cell-seekone-1.1.0 --help, and the only differnet parameter is :
--kit                          [choice]  The 10x or SeekOne kit and version separated by a colon (eg: 3prime:v3)
                                           * 3prime:v2
                                           * 3prime:v3
                                           * 3prime:v4
                                           * 5prime:v1
                                           * 5prime:v2
                                           * 5prime:v3
                                           * multiome:v1
                                           * visium:v1
                                           * visium_hd:v1
                                           * flseekone:DDv1
                                           * 3seekone:DDv2
                                           * 5seekone:DDv2
When the SeekOne DD single cell is 3`-library, it should be set "--kit 3seekone:DDv2", and if 5`-library, it should be set "--kit 5seekone:DDv2", and if SeekOne® DD Single-Cell Full-Length Transcriptome, set as "--kit flseekone:DDv1".
