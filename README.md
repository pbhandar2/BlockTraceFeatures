# BlockTraceFeatures
This repository contains features generated from publicly available block traces. 

1. CloudPhysics 
2. Tencent 
3. MSR 

## Features
Given a block trace, size of a Logical Block Address (LBA) and the size of a page the following features are generated at 30 minute intervals. 


| Feature      | Description |
| ----------- | ----------- |
| block_req_count        | number of block requests       |
| read_block_req_count   | number of  read block requests |
| write_block_req_count  | number of write block requests |
| seq_count             | number of sequential block requests | 
| read_seq_count | number of sequentiral read block requests |
| write_seq_count | number of sequential write block requests |
| range | the difference between the maximum and minimum byte offset accessed | 
| page_access_count | number of pages accessed | 
| read_page_access_count | number of pages read |
| write_page_access_count | number of pages written | 
| misalignment_sum | the sum of bytes by which block requests were not page aligned |
| read_misalignment_sum | the sum of bytes by which read block requests were not page aligned | 
| write_misalignment_sum | the sum of bytes by which write block requests were not page aligned | 



