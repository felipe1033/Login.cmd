@echo off 
title sistema de login
: home
cls
echo /========================================\
echo :  coloque Seu usuario e senha para poder :
echo : entrar no computador.                   :  
echo \========================================/
echo.
set/p user="Usuario : "
if "%user%"== "HIFUZION.bat" goto pass
msg * ERRO! Usuario invalido.
goto home
:pass
set/p pwd="Senha privada: "
if "%pwd%"== "52xmax01" Bem-Vindo %user%! Hoje eh %date%. &exit
msg * ERRO! Senha privada invalida ou nao reconhecida.
goto pass
