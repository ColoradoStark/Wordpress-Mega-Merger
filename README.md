# Wordpress-Mega-Merger

![Version](https://img.shields.io/github/v/release/ColoradoStark/Wordpress-Mega-Merger)

## Why did I make this?

This repository was made to solve this specific use case:  Maybe you made a bunch of websites, maybe you bought a few websites.  But now, you have 5 or more websites that don't have a CMS or have different CMS, and you want to consolidate all of your sites into one new domain and manage all of the content via CMS.  

## What exactly does this do?

Every page from the sites being merged will be preserved. Every link will still resolve.  Every URL will be 301 redirected to the new site. And you can still control all pages on the site via a CMS. 

## How does it do it?

To achieve this, it uses 2 CMS systems: Wordpress and Caddy Templates.  Any new pages you make will be done with wordpress.  All of the old sites you are merging will have the old pages plus custom headers and footers updated as plain HTML files.  They will be included the same way PHP includes or Apache SHTML includes work but you don't need new special URLs like `somepage.php` or `somepage.shtml` it will use includes as a plain HTML page.

## What do I need to know how to use to work this?
Ubuntu, Docker, Docker-Compose, Caddy

## How do I run this?
1. On an Ubuntu server with Docker and Docker-Compose installed clone the repo
2. type `cd Wordpress-Mega-Merger`
3. type `docker-compose up`


