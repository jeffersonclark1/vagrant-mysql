# VAGRANT MYSQL
## _Infrastructure and Cloud Computing - MBA ES21_

## Desafio

> Subir uma máquina virtual, usando Vagrant, com MySQL instalado e que esteja acessível no host da máquina na porta 3306.

## Tech

Tecnologias utilizadas

- [MySQL](https://www.mysql.com/) - Banco de dados.
- [Vagrant](https://www.vagrantup.com/) - Software das virtualizações
- [Ubuntu](https://ubuntu.com/) - Sistema operacional.
- [Virtual Box](https://www.virtualbox.org/) - Máquina virtual

## Instalação


```sh
mkdir vagrant && cd vagrant
git clone https://github.com/jeffersonclark1/vagrant-mysql.git
vagrant up
vagrant ssh
```

- User : root 
- Password : root


```sh
mysql -u root -p
CREATE DATABASE dbname;
USE dbname;
CREATE TABLE example ( id smallint unsigned not null auto_increment, name varchar(20) not null, constraint pk_example primary key (id) );
INSERT INTO example ( id, name ) VALUES ( null, 'Sample data' );
SELECT * FROM example;
```

## License

MIT

**Let's GO**
