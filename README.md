# Batch-data-pipelines-in-AWS
1. Yêu cầu:
- Docker installed(version 20.10.17, build 100c701)
- psql installed
- AWS CLI installed and basic config (region, access key, secret key,...)

2. Xây cơ sở hạ tầng trên AWS:
- ./setup_infra.sh {new-s3-bucket-name}
- Các tài nguyên sau được tạo:
  + new-s3-bucket-name là 1 data lake.
  + 1 cụm RedShift như 1 data warehouse.
  + 1 cụm EMR để biến đổi dữ liệu.
  + 1 EC2 chạy Airflow, Metabase

3. Hủy cơ sở hạ tầng đã tạo (phí khoảng $0.5/giờ)
- ./tear_down_infra.sh {new-s3-bucket-name}

4. Sơ đồ:
![SDE](https://user-images.githubusercontent.com/105615288/187131318-0f6a7d47-f4f2-49e0-aee4-1608ffefbe14.png)



[bổ sung sau...]
