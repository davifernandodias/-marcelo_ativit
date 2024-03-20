CREATE TABLE IF NOT EXISTS contatos (
    id INTEGER PRIMARY KEY,
    nome TEXT,
    email TEXT,
    telefone TEXT,
    grupo TEXT,
    favorito BOOLEAN
);

INSERT INTO contatos (nome, email, telefone, grupo, favorito) VALUES
('Davi1', 'davi1@email.com', '111111111', 'trabalho', 0),
('Davi2', 'davi2@email.com', '222222222', 'trabalho', 0),
('Davi3', 'davi3@email.com', '333333333', 'escola', 0),
('Davi4', 'davi4@email.com', '444444444', 'família', 0),
('Davi5', 'davi5@email.com', '555555555', 'amigo', 0),
('Davi6', 'davi6@email.com', '666666666', 'trabalho', 0),
('Davi7', 'davi7@email.com', '777777777', 'trabalho', 0),
('Davi8', 'davi8@email.com', '888888888', 'família', 0),
('Davi9', 'davi9@email.com', '999999999', 'escola', 0),
('Davi10', 'davi10@email.com', '1010101010', 'amigo', 0),
('Davi11', 'davi11@email.com', '1111111111', 'trabalho', 0),
('Davi12', 'davi12@email.com', '1212121212', 'trabalho', 0),
('Davi13', 'davi13@email.com', '1313131313', 'família', 0),
('Davi14', 'davi14@email.com', '1414141414', 'escola', 0),
('Davi15', 'davi15@email.com', '1515151515', 'amigo', 0),
('Davi16', 'davi16@email.com', '1616161616', 'trabalho', 0),
('Davi17', 'davi17@email.com', '1717171717', 'trabalho', 0),
('Davi18', 'davi18@email.com', '1818181818', 'família', 0),
('Davi19', 'davi19@email.com', '1919191919', 'escola', 0),
('Davi20', 'davi20@email.com', '2020202020', 'amigo', 0),
('Davi21', 'davi21@email.com', '2121212121', 'trabalho', 0),
('Davi22', 'davi22@email.com', '2222222222', 'trabalho', 0),
('Davi23', 'davi23@email.com', '2323232323', 'família', 0),
('Davi24', 'davi24@email.com', '2424242424', 'escola', 0),
('Davi25', 'davi25@email.com', '2525252525', 'amigo', 0),
('Davi26', 'davi26@email.com', '2626262626', 'trabalho', 0),
('Davi27', 'davi27@email.com', '2727272727', 'trabalho', 0),
('Davi28', 'davi28@email.com', '2828282828', 'família', 0),
('Davi29', 'davi29@email.com', '2929292929', 'escola', 0),
('Davi30', 'davi30@email.com', '3030303030', 'amigo', 0),
('Davi31', 'davi31@email.com', '3131313131', 'trabalho', 0),
('Davi32', 'davi32@email.com', '3232323232', 'trabalho', 0),
('Davi33', 'davi33@email.com', '3333333333', 'família', 0),
('Davi34', 'davi34@email.com', '3434343434', 'escola', 0),
('Davi35', 'davi35@email.com', '3535353535', 'amigo', 0),
('Davi36', 'davi36@email.com', '3636363636', 'trabalho', 0),
('Davi37', 'davi37@email.com', '3737373737', 'trabalho', 0),
('Davi38', 'davi38@email.com', '3838383838', 'família', 0),
('Davi39', 'davi39@email.com', '3939393939', 'escola', 0),
('Davi40', 'davi40@email.com', '4040404040', 'amigo', 0),
('Davi41', 'davi41@email.com', '4141414141', 'trabalho', 0),
('Davi42', 'davi42@email.com', '4242424242', 'trabalho', 0),
('Davi43', 'davi43@email.com', '4343434343', 'família', 0),
('Davi44', 'davi44@email.com', '4444444444', 'escola', 0),
('Davi45', 'davi45@email.com', '4545454545', 'amigo', 0),
('Davi46', 'davi46@email.com', '4646464646', 'trabalho', 0),
('Davi47', 'davi47@email.com', '4747474747', 'trabalho', 0),
('Davi48', 'davi48@email.com', '4848484848', 'família', 0),
('Davi49', 'davi49@email.com', '4949494949', 'escola', 0),
('Davi50', 'davi50@email.com', '5050505050', 'amigo', 0);


SELECT * FROM contatos WHERE nome = 'Davi1';
SELECT * FROM contatos WHERE email = 'davi1@email.com';

SELECT * FROM contatos WHERE grupo = 'trabalho';

SELECT * FROM contatos WHERE favorito = 1;

UPDATE contatos SET telefone = '111111111' WHERE id = 1;

DELETE FROM contatos WHERE nome = 'Davi40';


ALTER TABLE contatos ADD COLUMN favorito BOOLEAN;
