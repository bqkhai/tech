#### Monolithic: 1 server chứa tất cả

#### Phân cụm cluster: Nhiều server con

#### Phân cụm cluster + Load balancer: Load balancer --> Nhiều server con --> 1 database

#### Phân cụm cluster + Load balancer: Load balancer --> Nhiều server con --> 2 database (đọc và ghi)
- Server db đọc >> Server db ghi (Master ~ Slave)
- Đồng bộ 2 database: Mysql sync_binlog, Mysql replication, database middleware: my cat, 

#### Phân cụm cluster + Load balancer: Load balancer --> Nhiều server con --> 2 database (đọc và ghi)
- Server db đọc >> Server db ghi (Master ~ Slave)
- Thêm Search engine: Elastic search ...
- Đồng bộ các con db

#### Phân cụm cluster + Load balancer: Load balancer --> Nhiều server con --> 2 database (đọc và ghi)
- Server db đọc >> Server db ghi (Master ~ Slave)
- Thêm Search engine: Elastic search ...
- Cache: Redis, Memcached ---> Phục vụ việc đọc
- Đồng bộ các con db


#### ==> Hệ thống: CCU, đồng thời cao, độ trễ thấp, sẵn sàng cao (HA)

Triển khai High Availability:
- Primary + Backup
- Primary + Secondary
- Primary + Primary
