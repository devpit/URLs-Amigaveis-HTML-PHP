# **URLs Amigáveis para Projetos HTML e PHP**

*Esta abordagem ajuda a criar URLs mais amigáveis para os usuários em projetos que envolvem códigos HTML e PHP. URLs amigáveis simplificam a experiência do usuário e o processamento de URLs pelo servidor Apache, permitindo uma estrutura de URLs mais organizada e fácil de gerenciar.*

## **Tecnologias Compatíveis**

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![PHP](https://img.shields.io/badge/PHP-777BB4?style=for-the-badge&logo=php&logoColor=white)

## **Benefícios**

- *URLs mais amigáveis para o usuário.*
- *Simplificação do processamento de URLs pelo servidor Apache.*
- *Estrutura de URLs mais organizada e fácil de gerenciar.*

## **Como Usar**

*Para implementar URLs amigáveis em projetos HTML e PHP, siga os seguintes passos:*

1. **Configuração do Apache**: *Certifique-se de que o servidor Apache esteja configurado para manipular URLs amigáveis. Você pode fazer isso alterando as configurações no arquivo `.htaccess`.*

- *Caso não tenha um arquivo `.htaccess` pré configurado, basta criar um.*
- *Dentro do arquivo `.htaccess` insira o codigo a seguir.*

  ```bash
  RewriteEngine on
  RewriteCond %{REQUEST_FILENAME} !-d
  RewriteCond %{REQUEST_FILENAME}\.html -f
  RewriteRule ^(.*)$ $1.html

  RewriteEngine On
  RewriteCond %{REQUEST_FILENAME} !-d
  RewriteCond %{REQUEST_FILENAME}\.php -f
  RewriteRule ^(.*)$ $1.php [NC,L]
  ```

- *Ou baixe o código nos deixado nos arquivos deste repositório.*

2. **Estrutura de URLs**: *Crie uma estrutura de URLs organizada para o seu projeto HTML e PHP. Por exemplo, você pode usar URLs como `/pagina` em vez de `/pagina.html` ou `/pagina.php`.*

3. **Links Amigáveis**: *Ao criar links em seu site, use URLs amigáveis em vez de URLs com extensões. Isso tornará a experiência do usuário mais agradável.*

## **Exemplo**

*Aqui está um exemplo de como a estrutura de URLs pode parecer:*

- *URL Amigável (HTML): `https://seusite.com/pagina`*
- *URL Amigável (PHP): `https://seusite.com/pagina`*
- *URL Antiga (HTML): `https://seusite.com/pagina.html`*
- *URL Antiga (PHP): `https://seusite.com/pagina.php`*

## **Contribuição**

*Fique à vontade para contribuir com melhorias ou relatar problemas. Sua contribuição é bem-vinda!*
