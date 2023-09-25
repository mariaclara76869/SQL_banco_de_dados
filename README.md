# SQL_banco_de_dados
--01--
select * from tabela_paises;
![Captura de tela_2023-09-25_08-48-45](https://github.com/mariaclara76869/SQL_banco_de_dados/assets/131163181/cc31dcac-c3e3-4ea9-a494-0f1018a1c9d3)


--02--
select cidade from tabela_paises where pais = 'Brazil';
![Captura de tela_2023-09-25_08-51-32](https://github.com/mariaclara76869/SQL_banco_de_dados/assets/131163181/dec1f2a9-c81c-4b27-bec6-1ef954ef6e1c)


--03--
select cidade from tabela_paises where regiao = 'Ceara';
![Captura de tela_2023-09-25_08-51-49](https://github.com/mariaclara76869/SQL_banco_de_dados/assets/131163181/64899c8e-774c-48af-8458-9e64bb9995c1)

--04--
select count(*) as quantidade_regioes, regiao
from tabela_paises
where pais = 'China'
group by regiao;
![Captura de tela_2023-09-25_08-52-03](https://github.com/mariaclara76869/SQL_banco_de_dados/assets/131163181/df325329-38c7-4fca-9470-67e0b3e62ed7)

--05--
select distinct regiao, count(*) as quantidade_regioes
from tabela_paises
where pais = 'Canada'
group by regiao;
![Captura de tela_2023-09-25_08-52-20](https://github.com/mariaclara76869/SQL_banco_de_dados/assets/131163181/016e3e0a-3c98-4a16-bf4d-cf1790c10b9f)

--06--
select count (distinct pais) as total_paises
from tabela_paises;
![Captura de tela_2023-09-25_08-52-40](https://github.com/mariaclara76869/SQL_banco_de_dados/assets/131163181/b83966a4-5143-4096-a913-f90e5bb6977c)

--07--
select count (distinct cidade) as cidade_diferentes 
from tabela_paises
where pais = 'Brazil';
![Captura de tela_2023-09-25_08-52-53](https://github.com/mariaclara76869/SQL_banco_de_dados/assets/131163181/0c007502-27f6-4d10-9b8f-a0d512602f08)

--08--
select pais, count(regiao) as quantidade_regioes
from tabela_paises
group by pais;
![Captura de tela_2023-09-25_08-53-13](https://github.com/mariaclara76869/SQL_banco_de_dados/assets/131163181/6ff6d2ea-79f1-49e3-884c-37f6ef414081)

--09--
select count(*) as quantidade_pessoas
from tabela_paises
where nome
like 'João%';
![Captura de tela_2023-09-25_08-53-25](https://github.com/mariaclara76869/SQL_banco_de_dados/assets/131163181/0b40ace8-fff3-4e42-9531-710368ea43fd)

--10--
select count(*) as quantidades_john
from tabela_paises
where nome
like 'John%';
![Captura de tela_2023-09-25_08-53-36](https://github.com/mariaclara76869/SQL_banco_de_dados/assets/131163181/d5ac8d34-b480-4b11-a3c7-e52c4a82d6d8)

--11--
select distinct pais
from tabela_paises
order by pais;
![Captura de tela_2023-09-25_08-54-01](https://github.com/mariaclara76869/SQL_banco_de_dados/assets/131163181/f31f299d-5934-4caa-8395-9a6e47e6a337)
