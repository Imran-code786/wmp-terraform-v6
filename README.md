# wmp-terraform-v6

tfvars contain

1, Environment values
  env = "dev"

2, Instance Type

  instance_type = "t3.small"
  
3, Region

  region = "us-east-1"

4, Ports

   ports = {
      ssh = 22
      http  = 80
}

5, Apps details
    apps = {
      frontend = {
         instance_type  = "t3.small"
  }
}

6, Database details

    databases = {
       mysql = {
         instance_type  = "t3.medium"
  }
  
}

example:

env = "dev"

dns_domain = "example.com"

instance_type = "t3.small"

ports = {
ssh  = 22
http = 80
}

apps = {
frontend = {
instance_type = "t3.small"
port = 80
}

backend = {
instance_type = "t3.medium"
port = 8080
}
}