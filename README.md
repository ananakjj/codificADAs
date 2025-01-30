#Codificadas - Trabalho Final

CSS

<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    
    <title>Saga Star Wars</title>
    <style>
        /* Reset básico */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Arial', sans-serif;
            line-height: 1.6;
            background-color: #1a1a1a;
            color: #f4f4f4;
        }

        header {
            background-color: #000;
            color: #ffd700;
            padding: 20px 0;
            text-align: center;
            border-bottom: 3px solid #ffd700;
            position: relative;
        }

        header h1 {
            font-size: 2.5rem;
            font-weight: bold;
        }

        /* Imagem de fundo no header */
        header::before {
            content: "";
            background-image: url('https://i.imgur.com/3ZQZQ9M.png'); /* Estrela da Morte */
            background-size: cover;
            background-position: center;
            opacity: 0.3;
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            z-index: -1;
        }

        section {
            padding: 20px;
            margin: 20px auto;
            max-width: 800px;
            background-color: #2a2a2a;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.3);
        }

        h2 {
            color: #ffd700;
            margin-bottom: 15px;
            font-size: 2rem;
            border-bottom: 2px solid #ffd700;
            display: inline-block;
            padding-bottom: 5px;
        }

        p, li {
            font-size: 1.1rem;
            margin-bottom: 10px;
        }

        ul {
            list-style-type: square;
            padding-left: 20px;
        }

        table {
            width: 100%;
            border-collapse: collapse;
            margin-top: 15px;
            border-radius: 10px;
            overflow: hidden; /* Para arredondar os cantos da tabela */
        }

        table, th, td {
            border: 1px solid #ffd700;
        }

        th, td {
            padding: 10px;
            text-align: left;
        }

        th {
            background-color: #000;
            color: #ffd700;
            font-weight: bold;
        }

        tr:nth-child(even) {
            background-color: #333;
        }

        tr:hover {
            background-color: #444;
        }

        footer {
            background-color: #000;
            color: #ffd700;
            text-align: center;
            padding: 15px 0;
            margin-top: 30px;
            border-top: 3px solid #ffd700;
        }

        footer p {
            margin: 0;
            font-size: 0.9rem;
        }

        /* Imagens temáticas */
        .image-container {
            text-align: center;
            margin: 20px 0;
        }

        .image-container img {
            max-width: 80%; /* Define o mesmo tamanho para todas as imagens */
            height: auto; /* Mantém a proporção da imagem */
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.3);
        }

        /* Responsividade */
        @media (max-width: 768px) {
            header h1 {
                font-size: 2rem;
            }

            h2 {
                font-size: 1.5rem;
            }

            p, li {
                font-size: 1rem;
            }

            table {
                font-size: 0.9rem;
            }

            .image-container img {
                max-width: 100%; /* Aumenta o tamanho das imagens em dispositivos móveis */
            }
        }
    </style>
HTML 

</head>
<body>
    <header>
        <h1>Star Wars Saga</h1>
    </header>

    <section>
        <h2>A Saga que Atravessa Gerações</h2>
        <p>
            Star Wars é uma das sagas mais icônicas da história do cinema. Criada por George Lucas, a série cativou milhões de fãs ao redor do mundo, atravessando gerações e se tornando um fenômeno cultural. Desde o lançamento do primeiro filme em 1977, a saga expandiu-se para incluir trilogias, spin-offs, séries de TV, livros, quadrinhos e muito mais.
        </p>
        <p>
            Os fãs de Star Wars, conhecidos como "Star Wars Fans" ou "Jedi", são conhecidos por sua paixão e dedicação. Eles celebram a saga através de convenções, cosplays, fan arts e discussões intermináveis sobre o cânone e as teorias do universo expandido.
        </p>
        <div class="image-container">
            <img src="https://wallpapers.com/images/hd/4k-star-wars-logo-5binreit9du28bif.jpg" alt="Logo Star Wars">
        </div>
    </section>

    <section>
        <h2>A Inspiração de George Lucas</h2>
        <p>
            George Lucas se inspirou em diversas fontes para criar Star Wars:
        </p>
        <ul>
            <li><strong>Mitologia:</strong> A "Jornada do Herói", de Joseph Campbell, serviu como base para a estrutura narrativa da saga.</li>
            <li><strong>Filmes de Faroeste e Samurai:</strong> Cenas de ação e duelos foram influenciados por filmes de faroeste e obras de Akira Kurosawa.</li>
            <li><strong>Ficção Científica:</strong> Séries como "Flash Gordon" e "Buck Rogers" inspiraram o cenário espacial e a aventura.</li>
            <li><strong>Eventos Históricos:</strong> O conflito entre o Império e os Rebeldes reflete lutas entre o bem e o mal, inspiradas em eventos como a Guerra Fria.</li>
        </ul>
        <p>
            Com essas influências, Lucas criou uma saga que conquistou fãs de todas as idades e se tornou um grande marco na cultura pop.
        </p>
        <div class="image-container">
            <img src="https://wallpapers.com/images/hd/star-wars-characters-5mankml5qup4bj75.jpg" alt="Personagens Principais">
        </div>
    </section>

    <section>
        <h2>Ordem Cronológica da Saga</h2>
        <table>
            <thead>
                <tr>
                    <th>Nome do Filme</th>
                    <th>Ano Lançado</th>
                    <th>Personagens Principais</th>
                    <th>Bilheteria Mundial (USD)</th>
                    <th>Descrição Breve</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td>Star Wars: Episódio I - A Ameaça Fantasma</td>
                    <td>1999</td>
                    <td>Qui-Gon Jinn, Obi-Wan Kenobi, Anakin Skywalker</td>
                    <td>1.027 bilhão</td>
                    <td>O jovem Anakin Skywalker é descoberto e começa sua jornada para se tornar um Jedi.</td>
                </tr>
                <tr>
                    <td>Star Wars: Episódio II - Ataque dos Clones</td>
                    <td>2002</td>
                    <td>Anakin Skywalker, Padmé Amidala, Obi-Wan Kenobi</td>
                    <td>649 milhões</td>
                    <td>Anakin e Padmé se apaixonam enquanto a galáxia está à beira de uma guerra.</td>
                </tr>
                <tr>
                    <td>Star Wars: Episódio III - A Vingança dos Sith</td>
                    <td>2005</td>
                    <td>Anakin Skywalker, Obi-Wan Kenobi, Yoda</td>
                    <td>848 milhões</td>
                    <td>Anakin cai para o lado sombrio e se transforma em Darth Vader.</td>
                </tr>
                <tr>
                    <td>Star Wars: Episódio IV - Uma Nova Esperança</td>
                    <td>1977</td>
                    <td>Luke Skywalker, Leia Organa, Han Solo</td>
                    <td>775 milhões</td>
                    <td>Luke Skywalker começa sua jornada para se tornar um Jedi e derrotar o Império.</td>
                </tr>
                <tr>
                    <td>Star Wars: Episódio V - O Império Contra-Ataca</td>
                    <td>1980</td>
                    <td>Luke Skywalker, Leia Organa, Han Solo</td>
                    <td>538 milhões</td>
                    <td>O Império ataca os rebeldes, e Luke descobre a verdade sobre seu pai.</td>
                </tr>
                <tr>
                    <td>Star Wars: Episódio VI - O Retorno de Jedi</td>
                    <td>1983</td>
                    <td>Luke Skywalker, Leia Organa, Darth Vader</td>
                    <td>475 milhões</td>
                    <td>Luke confronta Darth Vader e o Imperador para salvar a galáxia.</td>
                </tr>
                <tr>
                    <td>Star Wars: Episódio VII - O Despertar da Força</td>
                    <td>2015</td>
                    <td>Rey, Finn, Poe Dameron</td>
                    <td>2.068 bilhões</td>
                    <td>Uma nova ameaça surge, e Rey descobre sua conexão com a Força.</td>
                </tr>
                <tr>
                    <td>Star Wars: Episódio VIII - Os Últimos Jedi</td>
                    <td>2017</td>
                    <td>Rey, Luke Skywalker, Kylo Ren</td>
                    <td>1.333 bilhão</td>
                    <td>Rey treina com Luke enquanto a Resistência luta pela sobrevivência.</td>
                </tr>
                <tr>
                    <td>Star Wars: Episódio IX - A Ascensão Skywalker</td>
                    <td>2019</td>
                    <td>Rey, Kylo Ren, Finn</td>
                    <td>1.074 bilhão</td>
                    <td>A saga Skywalker chega ao seu clímax com uma batalha final contra o Imperador Palpatine.</td>
                </tr>
            </tbody>
        </table>
    </section>

    <section>
        <h2>A Trilha Sonora da Saga</h2>
        <p>
            A trilha sonora de Star Wars, composta por John Williams, é tão icônica quanto a própria saga. Algumas das faixas mais famosas incluem:
        </p>
        <ul>
            <li><strong>Main Title (Tema Principal):</strong> A música de abertura que acompanha o texto rolante no início de cada filme.</li>
            <li><strong>The Imperial March (Marcha Imperial):</strong> O tema associado a Darth Vader e ao Império Galáctico.</li>
            <li><strong>Princess Leia's Theme:</strong> O tema da Princesa Leia, cheio de melodia e emoção.</li>
            <li><strong>Duel of the Fates:</strong> A música épica que acompanha o duelo entre Qui-Gon Jinn, Obi-Wan Kenobi e Darth Maul em "A Ameaça Fantasma".</li>
            <li><strong>Binary Sunset:</strong> A melodia tocada durante o pôr do sol em Tatooine, simbolizando a jornada de Luke Skywalker.</li>
        </ul>
        <div class="image-container">
            <img src="https://wallpapers.com/images/hd/star-wars-death-star-lobjmgq0es7whc97.jpg" alt="Estrela da Morte">
        </div>
    </section>

    <footer>
        <p>&copy; 2023 Star Wars Saga. Todos os direitos reservados.</p>
    </footer>
</body>
</html>
