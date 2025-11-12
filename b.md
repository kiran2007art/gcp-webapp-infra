gcloud compute instances create webapp-vm \
    --zone=us-east4-c \
    --machine-type=e2-medium \
    --image-family=debian-12 \
    --image-project=debian-cloud \
    --boot-disk-size=10GB \
    --disk name=webapp-disk \
    --tags=http-server \
    --metadata startup-script='#! /bin/bash
        apt update
        apt install -y nginx
        systemctl enable nginx
        systemctl start nginx'
