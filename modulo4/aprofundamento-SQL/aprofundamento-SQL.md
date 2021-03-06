<h1 align="center">Aprofundamento SQL</h1>

<div id= "top" align="center" ><img src="https://user-images.githubusercontent.com/94838711/161864744-eb5b178c-f854-46a0-bc1c-8dd28971754f.jpg" width="650px"/>
</div>

<p align="center">
  <a href="#1">Exercício 01</a> &#xa0;|&#xa0; 
  <a href="#2">Exercício 02</a> &#xa0;|&#xa0; 
  <a href="#3">Exercício 03</a> &#xa0;|&#xa0;
  <a href="#4">Exercício 04</a> &#xa0;|&#xa0;
  <a href="#5">Exercício 05</a>  &#xa0;|&#xa0;
  <a href="#6">Exercício 06</a> 
</p>

<h2 id="1" >✏️ EXERCÍCIO 01 </h2>

<p>A) ALTER TABLE Actor DROP COLUMN salary; O comando vai deletar a coluna de "salary".</p>

<p>B) ALTER TABLE Actor CHANGE gender sex VARCHAR(6); O comando vai mudar o bome da coluna de "gender" para "sex".</p>

<p>C) ALTER TABLE Actor CHANGE gender gender VARCHAR(255); O comando vai mudar a coluna "gender" para poder ter mais caracteres.</p>

<p>D) ALTER TABLE Actor CHANGE gender gender VARCHAR(100) NOT NULL;</p>


<h2 id="2">✏️ EXERCÍCIO 02 </h2>

<p>A) UPDATE Actor 
SET name = "Ju Paes" 
WHERE id = "003";</p>

<p>B) UPDATE Actor
SET name="JULIANA PAES" 
WHERE name="Juliana Paes";

UPDATE Actor  SET name="Juliana Paes" WHERE name="JULIANA PAES";</p>

<p>C) UPDATE Actor 
SET name = "Julio Paes", 
birth_date = "1956-05-10",
salary = 450000,
gender = "male" 
WHERE id = "005";</p>

<p>D) O fato do id não existir não permitirá que as linhas sejam atualizadas.</p>

<h2 id="3">✏️ EXERCÍCIO 03  </h2>

<p>A) DELETE FROM Actor WHERE name = "Fernanda Montenegro";</p>

<p>B) DELETE FROM Actor WHERE gender = "male" AND salary > 1000000;</p>

<h2 id="4">✏️ EXERCÍCIO 04 </h2>

<p>A) SELECT MAX(salary) FROM Actor;</p>

<p>B) SELECT MIN(salary) FROM Actor WHERE gender = "female";</p>

<p>C) SELECT COUNT(*) FROM Actor WHERE gender = "female";</p>

<p>D) SELECT SUM(salary) FROM Actor;</p>


<h2 id="5">✏️ EXERCÍCIO 05 </h2>

<p>A) SELECT COUNT(), gender FROM Actor GROUP BY gender; A query vai separar os atores por gênero e somar a quantidade de cada um.</p>

<p>B) SELECT id, name FROM Actor ORDER BY name DESC;</p>

<p>C) SELECT * FROM Actor ORDER BY salary ASC;</p>

<p>D) SELECT * FROM Actor ORDER BY salary DESC LIMIT 3;</p>

<p>E) SELECT AVG(salary), gender FROM Actor GROUP BY gender;</p>


<h2 id="6">✏️ EXERCÍCIO 06 </h2>

<p>A) ALTER TABLE Movie ADD COLUMN playing_limit_date DATE;</p>

<p>B) ALTER TABLE Movie CHANGE rating rating FLOAT NOT NULL;</p>

<p>C) UPDATE Movie SET playing_limit_date = "2021-04-02" WHERE id = "003";
UPDATE Movie SET playing_limit_date = "2020-05-20" WHERE id = "004";</p>

<p>D)Foi atualizado sem erros porém as linhas não forma alteradas.</p>