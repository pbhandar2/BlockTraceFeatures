# BlockTraceFeatures
This repository contains features generated from publicly available block traces. 

1. CloudPhysics 
2. Tencent 
3. MSR 

## Features
Given a block trace, size of a Logical Block Address (LBA) and the size of a page the following features are generated at 30 minute intervals. 


| Feature                     | Unit | Status | Description                                                          |
| --------------------------- | ---- | ------ | -------------------------------------------------------------------- |
| block_req_count             | -    | Done   | number of block requests                                             |
| read_block_req_count        | -    | Done   | number of read block requests                                        |
| write_block_req_count       | -    | Done   | number of write block requests                                       |
| write_block_req_split       | -    | Done   | fraction of block requests that were writes                          |
| io_request_size_sum         | byte | Done   | total IO requested                                                   |
| read_io_request_size_sum    | byte | Done   | total read IO requested                                              |
| write_io_request_size_sum   | byte | Done   | total write IO requested                                             |
| write_io_request_size_split | byte | Done   | fraction of IO that were writes                                      |
| page_access_count           | -    | Done   | number of pages accessed                                             |
| read_page_access_count      | -    | Done   | pages read                                                           |
| write_page_access_count     | -    | Done   | pages written                                                        |
| write_page_access_split     | -    | Done   | fraction of pages accessed that were writes                          |
| seq_count                   | -    | Done   | number of sequential block requests                                  |
| read_seq_count              | -    | Done   | number of sequential read block requests                             |
| write_seq_count             | -    | Done   | number of sequential write block requests                            |
| write_seq_split             | -    | Done   | fraction of sequential block requests that are writes                |
| range                       | byte | Done   | difference between the maximum and minimum byte offset accessed      |  
| read_range                  | byte | Done   | difference between the maximum and minimum byte offset read          |  
| write_range                 | byte | Done   | difference between the maximum and minimum byte offset written       |
| misalignment_sum            | byte | Done   | the sum of bytes by which block requests were not page aligned       |
| read_misalignment_sum       | byte | Done   | the sum of bytes by which read block requests were not page aligned  |
| write_misalignment_sum      | byte | Done   | the sum of bytes by which write block requests were not page aligned |
