provider "aws" {
    region= "ap-south-1"
}
 resource "aws_instance" "terraform_instance" {
    ami = "ami-02b49a24cfb95941c"
    instance_type = "t2.micro"
    
        key_name = "AWS2024"
    tags= {
        name="instance_terraform"
    }
    
