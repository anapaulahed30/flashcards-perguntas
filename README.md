function criaCartao(categoria, pergunta, resposta) {
    let container = document.getElementById('container')
    let cartao = document.createElement('article')
    cartao.className = 'cartao'

    cartao.innerHTML = `
    <div class="cartao__conteudo">
        <h3>${categoria}</h3>
        <div class="cartao__conteudo__pergunta">
            <p><strong>Pergunta:</strong> ${pergunta}</p>
        </div>
        <div class="cartao__conteudo__resposta">
            <p><strong>Resposta:</strong> ${resposta}</p>
        </div>
    </div>
    `

    let respostaEstaVisivel = false

    function viraCartao() {
        respostaEstaVisivel = !respostaEstaVisivel
        cartao.classList.toggle('active', respostaEstaVisivel)
    }
    cartao.addEventListener('click', viraCartao)

    container.appendChild(cartao)
}

// 🚗 Veículos
criaCartao("🚗 Veículos", "Qual é a função do catalisador em um automóvel?", "Reduzir a emissão de poluentes.");
criaCartao("🚗 Veículos", "O que significa a sigla “ABS” nos sistemas de freios?", "Sistema de freio antitravamento.");
criaCartao("🚗 Veículos", "Qual é a diferença entre motor a gasolina e motor diesel?", "Motores a diesel são mais eficientes e duráveis, mas mais poluentes.");
criaCartao("🚗 Veículos", "O que caracteriza um carro elétrico?", "Funcionamento com motor elétrico e baterias recarregáveis.");
criaCartao("🚗 Veículos", "Como funciona o sistema de transmissão automática?", "Troca de marchas é feita automaticamente sem intervenção do motorista.");
criaCartao("🚗 Veículos", "Que tipo de energia é usada por veículos híbridos?", "Combinação de energia elétrica e combustível fóssil.");
criaCartao("🚗 Veículos", "Qual a vantagem da aerodinâmica no desempenho de um veículo?", "Reduz a resistência do ar, melhora a velocidade e economia de combustível.");

// 🎨 Artistas
criaCartao("🎨 Artistas", "Quem pintou a obra “Guernica”?", "Pablo Picasso.");
criaCartao("🎨 Artistas", "Qual artista ficou conhecido por cortar sua própria orelha?", "Vincent van Gogh.");
criaCartao("🎨 Artistas", "Que cantor(a) brasileiro(a) é conhecido como o “Rei” da música romântica?", "Roberto Carlos.");
criaCartao("🎨 Artistas", "Qual o nome verdadeiro de Lady Gaga?", "Stefani Joanne Angelina Germanotta.");
criaCartao("🎨 Artistas", "Que movimento artístico foi liderado por Salvador Dalí?", "Surrealismo.");
criaCartao("🎨 Artistas", "Qual artista brasileiro é conhecido por pintar figuras geométricas coloridas e foi destaque na Pop Art?", "Romero Britto.");
criaCartao("🎨 Artistas", "Qual cantor(a) venceu mais prêmios Grammy na história?", "Beyoncé.");
criaCartao("🎨 Artistas", "Em que país nasceu Pablo Picasso?", "Espanha.");

// ⚽ Esportes
criaCartao("⚽ Esportes", "Qual país venceu a Copa do Mundo de 2018?", "França.");
criaCartao("⚽ Esportes", "Quantos jogadores há em um time de vôlei?", "Seis jogadores.");
criaCartao("⚽ Esportes", "Qual é o nome da competição internacional mais importante do atletismo?", "Campeonato Mundial de Atletismo.");
criaCartao("⚽ Esportes", "Em que esporte se destacaram Michael Jordan e LeBron James?", "Basquete.");
criaCartao("⚽ Esportes", "O que é um Grand Slam no tênis?", "Conjunto dos quatro torneios mais importantes do tênis mundial.");
criaCartao("⚽ Esportes", "Qual é a distância oficial de uma maratona?", "42,195 km.");
criaCartao("⚽ Esportes", "Quem é considerado o maior nadador olímpico da história?", "Michael Phelps.");

// 🧬 Biologia
criaCartao("🧬 Biologia", "Qual é a molécula responsável por carregar o código genético?", "O DNA.");
criaCartao("🧬 Biologia", "O que são mitocôndrias e qual sua função na célula?", "Organelas que produzem energia (ATP) para a célula.");
criaCartao("🧬 Biologia", "O que diferencia um ser vivo autotrófico de um heterotrófico?", "Autotróficos produzem seu próprio alimento; heterotróficos dependem de outros seres.");
criaCartao("🧬 Biologia", "Onde ocorre a fotossíntese nas plantas?", "Nos cloroplastos das células vegetais.");
criaCartao("🧬 Biologia", "O que é DNA e qual sua importância?", "Ácido desoxirribonucleico, responsável pela hereditariedade.");
criaCartao("🧬 Biologia", "Qual a principal função do sistema imunológico?", "Proteger o organismo contra agentes patogênicos.");
criaCartao("🧬 Biologia", "O que caracteriza os mamíferos?", "Presença de glândulas mamárias e pelos.");
criaCartao("🧬 Biologia", "Como se chama o processo pelo qual uma célula se divide em duas?", "Mitose.");
