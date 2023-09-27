# Sentinel Dashboard Docker

## Quick Start

Run the following command：


* Run With docker

  ```
  sh docker run -p 8858:8858 -it bladex/sentinel-dashboard-docker
  ```

* Run With docker-compose

  ```
  sh docker-compose up
  ```

* Open the Sentinel Dashboard console in your browser

  link：http://127.0.0.1:8858/


## Common property configuration

| name                         | description                            | option                         |
| ---------------------------- | -------------------------------------- | ------------------------------ |
| SERVER_PORT                  | server启动的端口                         | 8858                           |
| PROJECT_NAME                 | 项目名称                                 | sentinel-dashboard             |
| USERNAME                     | dashboard登陆用户名                      | 默认sentinel                    |
| PASSWORD                     | dashboard登陆密码                        | 默认sentinel                    |
