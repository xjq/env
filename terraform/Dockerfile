FROM opensuse:leap
WORKDIR /env
RUN zypper in -y wget unzip aaa_base-extras
RUN wget https://releases.hashicorp.com/terraform/0.12.1/terraform_0.12.1_linux_amd64.zip
RUN unzip terraform_0.12.1_linux_amd64.zip
RUN chmod u+x terraform
RUN mv terraform /usr/bin/terraform
CMD "/bin/bash"
