# BlockTraceFeatures
This repository contains features generated from publicly available block traces. 

1. CloudPhysics 
2. Tencent 
3. MSR 

## Features
Given a block trace, size of a Logical Block Address (LBA) and the size of a page the following features are generated at 30 minute intervals. 


| Feature                     | Unit | Status | Description                                           |
| --------------------------- | ---- | ------ | ----------------------------------------------------- |
| block_req_count             | -    | Done   | number of block requests                              |
| read_block_req_count        | -    | Done   | number of read block requests                         |
| write_block_req_count       | -    | Done   | number of write block requests                        |
| write_block_req_split       | -    | Done   | fraction of block requests that were writes           |
| io_request_size_sum         | byte | Done   | total IO requested                                    |
| read_io_request_size_sum    | byte | Done   | total read IO requested                               |
| write_io_request_size_sum   | byte | Done   | total write IO requested                              |
| write_io_request_size_split | byte | Done   | fraction of IO that were writes                       |
| page_access_count           | -    | Done   | number of pages accessed                              |
| read_page_access_count      | -    | Done   | pages read                                            |
| write_page_access_count     | -    | Done   | pages written                                         |
| write_page_access_split     | -    | Done   | fraction of pages accessed that were writes           |
| seq_count                   | -    | Done   | number of sequential block requests                   |
| read_seq_count              | -    | Done   | number of sequential read block requests              |
| write_seq_count             | -    | Done   | number of sequential write block requests             |
| write_seq_split             | -    | Done   | fraction of sequential block requests that are writes |



<!-- 
| block_req_count_split  | fraction of block requests that were writes | ratio |
| seq_count             | number of sequential block requests | frequency |
| read_seq_count | number of sequentiral read block requests | frequency |
| write_seq_count | number of sequential write block requests | frequency |
| page_access_count | number of pages accessed | frequency |
| read_page_access_count | number of pages read | frequency |
| write_page_access_count | number of pages written |  frequency |
| write_page_access_split | fraction of page accesses that were for writes | ratio | 
| misalignment_sum | the sum of bytes by which block requests were not page aligned | bytes |
| read_misalignment_sum | the sum of bytes by which read block requests were not page aligned | bytes | 
| write_misalignment_sum | the sum of bytes by which write block requests were not page aligned | bytes |
| misaligned_request_split | the fraction of block requests that were not page aligned | bytes |
| read_misaligned_request_split | the fraction of read block requests that were not page aligned | ratio |
| write_misaligned_request_split | the fraction of write block requests that were not page aligned | ratio |
| range | the difference between the maximum and minimum byte offset accessed | byte | -->



