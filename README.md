# Projet-S-curit-GL4
# Authentication and Network Services Configuration

## Part 1: Authentication with OpenLDAP, SSH, Apache, OpenVPN

### Section 1: OpenLDAP Configuration

#### 1.1 Configure an OpenLDAP server with 2 users and 2 groups.

#### 1.2 Add information, including x509 certificates, for all users.

#### 1.3 Successfully authenticate to the OpenLDAP server.

#### 1.4 Test the secure part of LDAP with ldaps and describe the various advantages.

### Section 2: SSH Authentication

#### 2.1 Enable SSH authentication via OpenLDAP.

#### 2.2 Restrict SSH access to users from the appropriate group in OpenLDAP.

#### 2.3 Test for an authorized and unauthorized user to SSH.

### Section 3: Apache Integration

#### 3.1 Configure Apache to use OpenLDAP authentication.

#### 3.2 Ensure web page access is limited to members of the appropriate group in OpenLDAP.

#### 3.3 Test for an authorized and unauthorized user on a chosen website.

### Section 4: OpenVPN Setup

#### 4.1 Install and configure OpenVPN to use OpenLDAP authentication.

#### 4.2 Successfully test VPN connection using OpenLDAP credentials.

#### 4.3 Test for an authorized and unauthorized client to initiate a VPN tunnel.

## Part 2: Network Services Management with DNS

### Section 1: DNS Server Configuration

#### 1.1 Configure a DNS server (Bind) on a separate machine.

#### 1.2 Add necessary DNS records for OpenLDAP, Apache, and OpenVPN servers.

### Section 2: Validation and Testing

#### 2.1 Test DNS resolution for each of the configured services.

#### 2.2 Ensure domain names associated with services are correctly resolved.

## Part 3: Authentication with Kerberos

### Section 1: Kerberos Server Configuration

#### 1.1 Install and configure a Kerberos server.

#### 1.2 Add principals and password policies for users.

### Section 2: Authentication with a Chosen Service

#### 2.1 Choose one of the services (OpenLDAP, SSH, Apache, or OpenVPN) to implement Kerberos authentication.

#### 2.2 Document and configure the chosen service to use Kerberos authentication.
