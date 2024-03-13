CREATE DATABASE IF NOT EXISTS agenda_contatos;

USE agenda_contatos;

CREATE TABLE IF NOT EXISTS contatos (
    id INT AUTO_INCREMENT PRIMARY KEY,
    nome VARCHAR(255) NOT NULL,
    email VARCHAR(255),
    telefone VARCHAR(20),
    grupo VARCHAR(255),
    favorito BOOLEAN DEFAULT 0
);

INSERT INTO contatos (nome, email, telefone, grupo, favorito) VALUES
("João", "joao@email.com", "123456789", "trabalho", 1),
("Maria", "maria@email.com", "987654321", "escola", 0),
("Pedro", "pedro@email.com", "456789123", "família", 0),
("Ana", "ana@email.com", "789123456", "amigo", 1);

SELECT * FROM contatos WHERE favorito = 1;

UPDATE contatos SET favorito = 1 WHERE nome = 'Maria';

UPDATE contatos SET favorito = 0 WHERE nome = 'Ana';
## DECLARANDO FAVORITOS
ALTER TABLE contatos ADD COLUMN favorito BOOLEAN DEFAULT 0;

UPDATE contatos SET favorito = 1 WHERE nome = 'João' OR nome = 'Ana';

SELECT * FROM contatos WHERE favorito = 1;

UPDATE contatos SET favorito = 1 WHERE nome = 'Maria';

UPDATE contatos SET favorito = 0 WHERE nome = 'Ana';
