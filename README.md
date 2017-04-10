This repository contains sources for RPMs that are used
to build Software Collections for CentOS by SCLo SIG.

This branch is for sclo-php56 packages (for rh-php56 SCL)


PHP 5.6 / EL-6

    build -bs *spec --define "scl rh-php56" --define "dist .el6"
    cbs add-pkg    sclo6-sclo-php56-sclo-candidate --owner=sclo  sclo-php56-php-pecl-http
    cbs add-pkg    sclo6-sclo-php56-sclo-testing   --owner=sclo  sclo-php56-php-pecl-http
    cbs add-pkg    sclo6-sclo-php56-sclo-release   --owner=sclo  sclo-php56-php-pecl-http
    cbs build      sclo6-sclo-php56-sclo-el6       <above>.src.rpm
    cbs tag-build  sclo6-sclo-php56-sclo-testing   <previous>

PHP 5.6 / EL 7

    build -bs *spec --define "scl rh-php56" --define "dist .el7"
    cbs add-pkg    sclo7-sclo-php56-sclo-candidate --owner=sclo  sclo-php56-php-pecl-http
    cbs add-pkg    sclo7-sclo-php56-sclo-testing   --owner=sclo  sclo-php56-php-pecl-http
    cbs add-pkg    sclo7-sclo-php56-sclo-release   --owner=sclo  sclo-php56-php-pecl-http
    cbs build      sclo7-sclo-php56-sclo-el7       <above>.src.rpm
    cbs tag-build  sclo7-sclo-php56-sclo-testing   <previous>


