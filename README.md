# BlockTraceFeatures
This repository contains features generated from publicly available block traces using a python block trace analysis framework, [pyCydonia](https://github.com/pbhandar2/pyCydonia)

1. CloudPhysics 
2. Tencent 
3. MSR 

## Features
Given a block trace, size of a Logical Block Address (LBA) and the size of a page the following features are generated for each 30 minute interval. 

### Basic.v1 

| Feature                           | Unit | Status | Description                                                                              |
| --------------------------------- | ---- | ------ | ---------------------------------------------------------------------------------------- |
| block_req_count                   | -    | Done   | number of block requests                                                                 |
| read_block_req_count              | -    | Done   | number of read block requests                                                            |
| write_block_req_count             | -    | Done   | number of write block requests                                                           |
| write_block_req_split             | -    | Done   | fraction of block requests that were writes                                              |
| io_request_size_sum               | byte | Done   | total IO requested                                                                       |
| read_io_request_size_sum          | byte | Done   | total read IO requested                                                                  |
| write_io_request_size_sum         | byte | Done   | total write IO requested                                                                 |
| write_io_request_size_split       | byte | Done   | fraction of IO that were writes                                                          |
| page_access_count                 | -    | Done   | number of pages accessed                                                                 |
| read_page_access_count            | -    | Done   | pages read                                                                               |
| write_page_access_count           | -    | Done   | pages written                                                                            |
| write_page_access_split           | -    | Done   | fraction of pages accessed that were writes                                              |
| seq_count                         | -    | Done   | number of sequential block requests                                                      |
| read_seq_count                    | -    | Done   | number of sequential read block requests                                                 |
| write_seq_count                   | -    | Done   | number of sequential write block requests                                                |
| write_seq_split                   | -    | Done   | fraction of sequential block requests that are writes                                    |
| range                             | byte | Done   | difference between the maximum and minimum byte offset accessed                          |  
| read_range                        | byte | Done   | difference between the maximum and minimum byte offset read                              |  
| write_range                       | byte | Done   | difference between the maximum and minimum byte offset written                           |
| misalignment_sum                  | byte | Done   | the sum of bytes by which block requests were not page aligned                           |
| read_misalignment_sum             | byte | Done   | the sum of bytes by which read block requests were not page aligned                      |
| write_misalignment_sum            | byte | Done   | the sum of bytes by which write block requests were not page aligned                     |  
| page_working_set_size             | byte | Done   | the size of the set of unique pages accessed                                             |  
| read_page_working_set_size        | byte | Done   | the size of the set of unique pages read                                                 |  
| write_page_working_set_size       | byte | Done   | the size of the set of unique pages written                                              |  
| write_page_working_set_size_split | -    | Done   | fraction of the working set size where data is written                                   |
| p_read_page_popularity            | -    | Done   | Percentiles(p)={1,5,10 .. 100} of the popularity of top-N% popular read pages            |  
| p_write_page_popularity           | -    | Done   | Percentiles(p)={1,5,10 .. 100} of the popularity of top-N% popular write pages           |
| p_read_block_request_size         | byte | Done   | Percentiles(p)={1,5,10 .. 100} of read block request sizes                               |
| p_write_block_request_size        | byte | Done   | Percentiles(p)={1,5,10 .. 100} of write block request sizes                              |
| p_jump_distance                   | byte | Done   | Percentiles(p)={1,5,10 .. 100} of the jump distance between block requests               |
| p_scan_length                     | byte | Done   | Percentiles(p)={1,5,10 .. 100} of the length of scans (new item or cache writes)         |  
| p_delta_read_page_popularity      | -    | Done   | Percentiles(p)={1,5,10 .. 100} of the change in popularity of pages from previous window |
| p_delta_write_page_popularity     | -    | Done   | Percentiles(p)={1,5,10 .. 100} of the change in popularity of pages from previous window |
