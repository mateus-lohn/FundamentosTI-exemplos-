# FundamentosTI-exemplos-
2)#!/bin/bash
eco ´´digite seu ano de nascimento 
read x
idadeparavoto=165
votar=((2021-$x))
if[ $votar -gt $idadepravoto ] 
then
echo ´´vc pode votar esse ano´´
else
echo ´´vc nao pode votar esse ano´´
fi

6)#!/bin/bash
echo ´´digite um valor´´
read N
variavel=0
if [ $N -gt $variavel]
then
for i in $(seq 1 $N)
do
echo ´´$i´´
done
else
echo ´´execute o codigo novamente e insira´´
fi

7)#!bin/bash
i=1
somavalores=0
maior=0
while [ $i -le 15 ]
do
echo ´´escreva o valor de $i produto´´
read valor
if [ $valor -gt $maior]
then
maior=$valor
fi
somavalores=$(($somavalores+$valor))
i=$(($i+1))
done
somavalores=$( bc <<< ´´scale=2; $somavalores/15´´)
echo´´o produto mais caro custa $maior reais´´
echo ´´a média de valor dos produtos é $somavalores´´
