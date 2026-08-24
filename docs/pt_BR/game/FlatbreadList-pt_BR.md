# A Lista de Promessas do The Native Pond

![flatbreadlist_background](/background/pt_BR/FBL-docs-bg-pt_BR.png)

> [!WARNING]
> 1. Todo o conteúdo desta lista são promessas vazias — não representa a apresentação final nem a implementação real.
> 2. Parte do conteúdo desta lista não foi discutida em reuniões da equipe.
> 3. Parte do conteúdo desta lista não passou por estudos de viabilidade.
> 4. Esta lista pode servir de orientação para obras derivadas e criações secundárias.
> 5. A equipe reserva todos os direitos de tomar medidas futuras em relação a esta lista, bem como o direito de interpretação final dela.

---

## 🎮 Controles

Movimento suave e boa câmera são partes essenciais para garantir que o jogo tenha jogabilidade. **O personagem precisa conseguir se mover!**

### Movimento

- O jogador controla o personagem para se mover pelo **mapa** e, em locais especiais (como a plataforma de pesca), pressiona um botão ou se posiciona em uma pequena área de coordenadas para **acionar** a animação de entrada naquele **local especial**.
- A **interação** com o jogo acontece por botões de toque (celular), teclado (PC) e controle; as teclas podem ser personalizadas.

### Câmera

- Nas áreas não especiais do mapa, usa-se a visão em **terceira pessoa**.
- Nas áreas especiais do mapa (como a plataforma de pesca), usa-se a visão em **primeira pessoa**, exibindo o interior da área (se houver).
- O mapa **se move** acompanhando a câmera.

---

## 🗺️ Sistema de Mapa

Debruce-se sobre a mesa e faça um **mapa** — o mapa tem de tudo!

### Zoom e orientação

- O mapa não **gira** junto com a câmera.
- O mapa pode dar **zoom**.
- O mapa segue a lógica de direção "**norte em cima, sul embaixo, oeste à esquerda, leste à direita**".

### Limites

- O mapa do jogo tem **limites**, ou seja, o jogador não consegue atravessar a **borda do mapa**.
- Quando o jogador tenta atravessar a borda, o jogo o **puxa de volta à força** e mostra a mensagem "* Uma sensação familiar toma conta de você — você parece ouvir: 'Vamos explorar a área à frente depois!' Mesmo sabendo que nunca poderá explorá-la depois, ainda quer tentar."
- Os limites podem ser **obstáculos naturais** evidentes (como grandes montanhas) ou **cercas artificiais** (como as paredes de arquitetura estilo Huizhou).

### Clima

- Os **tipos** de clima são:
	- Ensolarado.
	- Chuvoso.
	- Tempestade.
	- Nevando.
- As **mudanças** de clima podem ser determinadas por:
	1. Ajuste manual do jogador.
	2. Semelhança com o clima de determinada região.
	3. Probabilidade totalmente aleatória.

### Estações

- As estações mudam a cada **90 horas**.
- Os **tipos** de estação são:
	- Primavera.
	- Verão.
	- Outono.
	- Inverno.

### Câmera fotográfica

- O jogador pode **fotografar** em qualquer lugar (exceto na interface gráfica) pressionando uma tecla do teclado, tocando em um botão ou pressionando um botão do controle.
- Ao **fotografar**, o jogo exibirá uma cobertura de **luz branca** em tela cheia para representar a foto. Isso pode exigir um aviso de **epilepsia fotossensível** na tela inicial do jogo.
- Ao **fotografar**, o jogo automaticamente **captura** todos os elementos da tela (exceto os elementos da interface) e adiciona uma **moldura**.
- O jogo **salva** as fotos em uma **pasta específica** para facilitar o compartilhamento.

### O lago de pesca

- O lago de pesca é a área especial mais central do jogo, incluindo a **Plataforma de pesca**, o **Lago** e o **Barco**.

#### Plataforma de pesca

- Fica no extremo **sul** do lago.
- Quando o jogador **entra** nessa área especial, a câmera dá zoom automaticamente e muda para a visão em primeira pessoa; o personagem fica sentado e a interface visual da área é exibida.
- A plataforma de pesca serve para **pescar**.

#### Lago

- Fica no extremo **norte** do mapa.
- Quando o jogador **entra** nessa área especial, o personagem passa a **nadar**.

#### Barco

- Fica em **qualquer lugar** do lago (dependendo de onde o jogador estacionou o barco da última vez).
- Quando o jogador **entra** nessa área especial, o personagem passa a **pilotar** e a interface visual da área é exibida.
- O jogador pode pilotar o barco navegando pelo **lago**.

### Barraca

- Fica a **sudoeste** do centro do mapa.
- Quando o jogador **entra** nessa área especial, a câmera dá zoom automaticamente e muda para a visão em primeira pessoa, exibindo a interface visual da área.
- A barraca é o coração do **acampamento**.
- O **interior** e o **tamanho** da barraca podem seguir o design da barraca de *Robinson Crusoé*.

### Campo

- O campo fica a **sudeste** da barraca.
- Quando o jogador **entra** nessa área especial, a câmera dá zoom automaticamente e muda para a visão em primeira pessoa, exibindo a interface visual da área.
- O campo serve para **plantar**.

### Mercado

- O mercado fica a **leste** do mapa.
- Quando o jogador **entra** nessa área especial, a câmera dá zoom automaticamente e muda para a visão em primeira pessoa, exibindo a interface visual da área.
- O mercado serve para **comerciar**.

### Árvore

- Fica a **sudeste** da barraca.
- Quando o jogador **entra** nessa área especial, a câmera dá zoom automaticamente e muda para a visão em primeira pessoa; o personagem fica sentado.
- Às vezes (como no outono) aparecem **maçãs** na árvore. O jogador pode derrubá-las com uma **vara comprida** e **coletá-las**.
- Quando o jogador fica algum tempo (cerca de 1 minuto) **embaixo** da árvore, o jogo mostra um botão flutuante "Segure [W] para meditar"; ao pressionar W, tocar no botão ou pressionar o botão do controle, o jogador entra em **meditação**. Durante a **meditação**, o jogo exibe **efeitos visuais** em tela cheia (várias fórmulas de física), e há chance de ser **atingido por uma maçã**.

### Fogueira

- Fica a uma curta distância **a leste** da barraca.
- Quando o jogador **entra** nessa área especial, a câmera dá zoom automaticamente e muda para a visão em primeira pessoa, exibindo a interface visual da área.
- A fogueira pode ser **acesa** e fornece iluminação.
- A fogueira pode ser usada para **cozinhar**.

### Concha mágica

- O jogador pode pegar a **concha mágica** na **areia** da beira do lago.
- Quando o jogador **pega** a concha mágica, o personagem assume a posição de sopro e a câmera dá zoom automaticamente. Nesse momento, o jogador não pode se mover. A interface visual desse item especial também é exibida.
- A concha mágica tem 7 **tons** que o jogador pode soprar.
- A concha mágica tem várias **variedades**, cada uma com um **timbre** diferente.

### Caixa de correio

- Fica **ao sul** da barraca.
- Quando o jogador **entra** nessa área especial, a câmera dá zoom automaticamente e muda para a visão em primeira pessoa, exibindo a interface visual da área.
- A caixa de correio serve para **receber e enviar mensagens**.

---

## 🎣 Sistema de Pesca

Na **Plataforma de pesca**, o jogador pode usar uma **vara de pescar** para pescar.

### Espécies

- O **lago de pesca** do jogo pode render tanto **peixes de água salgada** quanto **peixes de água doce**. Além dos peixes, também é possível pescar **colecionáveis**.
	1. Isso pode ser determinado pela **plataforma de pesca** escolhida pelo jogador (por exemplo, uma plataforma na beira do mar só rende peixes de água salgada; uma plataforma na beira do lago só rende peixes de água doce).
	2. Isso pode ser determinado pela **probabilidade** de cada espécie (ou seja, em uma mesma plataforma na beira do mar, é possível pescar peixes de água salgada e de água doce conforme a probabilidade).
- A **probabilidade** de pescar cada espécie é determinada por:
	1. A probabilidade **real** de pescar cada espécie. Pode ser um intervalo de valores que se ajusta de acordo com vários fatores (como clima, estação etc.), em vez de ser fixo.
	2. Uma probabilidade totalmente **aleatória**.
- A **probabilidade** de pescar colecionáveis é determinada por:
	1. A **taxa de mordida** histórica do jogador.
	2. Uma **probabilidade** aleatória dentro de um intervalo fixo.
	3. Uma probabilidade totalmente **aleatória**.

### Taxa de mordida

Vale mencionar que a taxa de mordida se refere à probabilidade de o peixe **morder a isca**, não à probabilidade de finalmente pescar o peixe.

- A **taxa de mordida** do jogo é determinada em conjunto pelos seguintes fatores:
	- Se há isca no anzol do jogador.
	- Se o jogador fez ceva.
	- O tipo de isca no anzol.
	- O horário do jogo (por exemplo, dia ou noite).
	- Se a lanterna de cabeça está acesa à noite.
	- O clima do jogo.
	- A estação do jogo.
- A taxa de mordida também pode ser determinada por:
	1. A taxa de mordida histórica do jogador.
	2. Uma probabilidade totalmente aleatória.

### Taxa de captura

Como o nome sugere, a taxa de captura se refere à probabilidade de finalmente pescar o peixe.

- A **taxa de captura** do jogo é determinada em conjunto pelos seguintes fatores:
	- Se o peixe mordeu a isca.
	- O momento de erguer a vara (não pode ser cedo nem tarde demais).
	- A taxa de arrebentamento da linha de pesca.
	- O tamanho do anzol.

### Vara de pescar

- A vara de pescar é composta pela **vara**, a **bóia**, o **anzol** e a **linha de pesca**.
- Qualquer parte da vara tem **durabilidade**; quanto menor a durabilidade, maior a chance de a vara quebrar. Quando a vara quebra, é preciso **trocar** a parte danificada.

#### Vara

- A **vara** é um componente da **vara de pescar**.
- O jogador pode comprar varas pelo **sistema de comércio**, como a vara de 2,7 metros e a de 3,6 metros.
- Varas de comprimentos diferentes têm tempos de arremesso e de erguida diferentes.

#### Bóia

- A **bóia** é um componente da **vara de pescar**; o jogador decide se ergue a vara com base no **movimento da bóia**.
- O jogador pode comprar bóias pelo **sistema de comércio**, como a bóia comum e a bóia luminosa.
- O movimento da bóia quando cada espécie morde é diferente, tomando como referência o movimento real da bóia quando os peixes mordem.
- A bóia pode ser ajustada em **marcações** (ou seja, ajustando o peso do chumbo) para facilitar a observação.

#### Anzol

- O **anzol** é um componente da **vara de pescar** e a base para o jogador pescar.
- O jogador pode comprar anzóis pelo **sistema de comércio**, como o anzol pequeno e o anzol grande.
- O tamanho do anzol é o fator decisivo para pescar peixes grandes ou pequenos.
- O anzol pode receber **iscas**.

#### Linha de pesca

- A **linha de pesca** é um componente da **vara de pescar**.
- O jogador pode comprar linhas pelo **sistema de comércio**, como a linha comum nº 0.8 e a linha premium nº 2.0.
- Linhas diferentes têm **taxas de arrebentamento** diferentes, que podem ser determinadas em conjunto pelos seguintes fatores:
	- A qualidade da linha.
	- O tempo de uso ou a durabilidade da linha.

### Iscas

- O jogador pode comprar iscas pelo **sistema de comércio**, como a isca comum e as minhocas vermelhas.
- Se a isca comprada for em pó, é preciso transformá-la em isca passando por etapas como adicionar água e sovar a massa.
- Iscas diferentes têm **taxas de mordida** diferentes.
- Como item consumível, quando o jogador não tem iscas e a quantidade de conchas que possui (incluindo as conchas obtidas vendendo a pesca) não é suficiente para comprar um pacote de iscas, o jogo fará um reabastecimento gratuito pela **caixa de correio** no dia seguinte.

### Ceva

- O jogador pode comprar ceva pelo **sistema de comércio**, como borra de tofu fermentada e milho velho embebido em vinho.
- Ceva diferente tem **taxa de mordida** diferente.
- A ceva pode aumentar muito a taxa de mordida.

### Lanterna de cabeça

- O jogador pode comprar lanternas de cabeça pelo **sistema de comércio**, como a lanterna comum e a lanterna azul para pesca noturna.
- Lanternas diferentes têm **taxas de mordida** diferentes e efeitos visuais diferentes.
- À noite, a lanterna permite ver a superfície da água e a bóia.
- À noite, a lanterna pode assustar os peixes e reduzir a taxa de mordida.

### Colecionáveis

- Os colecionáveis se dividem principalmente em **garrafas à deriva**, **lembranças** e **fragmentos de história**.
- O jogador pode **obter** colecionáveis das seguintes formas:
	- Pescar.
	- Presentes do Cat.

#### Garrafa à deriva

- As garrafas à deriva contêm **cartas**.
- A maioria das cartas são **palavras de incentivo** para motivar o jogador.

#### Lembranças

- Algumas lembranças podem ser **expostas** na **barraca**.

#### Fragmentos de história

- Os fragmentos de história servem para guiar o jogador na descoberta da história dos **aldeões**.
- Quando todos os fragmentos de história são coletados, o jogador desbloqueia uma longa história para conhecer de forma completa e detalhada a história dos **aldeões**.

---

## 🍳 Sistema de Culinária

Prepare **comidas** e tente comê-las!

### Utensílios de cozinha

- Os utensílios de cozinha são compostos por três partes: o **fogareiro**, a **tábua de corte** e os **utensílios**.

#### Fogareiro

- O fogareiro serve para **aquecer** a comida.
- O fogareiro pode **ficar**:
	1. Dentro da barraca.
	2. Fora da barraca, mas perto dela.
- O fogareiro permite ao jogador colocar alguns **utensílios** (como a frigideira).
- Antes de usar o fogareiro, é preciso adicionar **combustível** a ele.
- O jogador precisa **controlar o fogo** para garantir que a comida feita seja comestível.

#### Tábua de corte

- A tábua de corte serve para **picar** a comida.
- A tábua de corte permite ao jogador colocar alguns **ingredientes** (como a acelga chinesa) e **comidas semiprontas**.
- O jogador pode usar alguns **utensílios** (como a faca de cozinha) para cortar na tábua.

#### Utensílios

- Os utensílios permitem ao jogador **manusear** os ingredientes com facilidade.
- Os utensílios incluem:
	- Panela grande.
	- Frigideira.
	- Cesto de vapor.
	- Tigela de porcelana.
	- Faca de cozinha.
	- Rolo de massa.

### Receitas

- O jogador pode preparar comidas seguindo as **receitas**. Em geral, seguindo a receita, a comida dá certo.
- O jogador também pode **não seguir** a receita e improvisar.

### Comidas

- Quando o jogador conclui todo o **processo de preparo**, obtém uma **comida**.
- O jogador pode preparar as seguintes comidas:
	- Macarrão simples (obtido em todo o processo, da farinha, passando por sovar a massa e cortar as tiras, até cozinhar na panela).
	- Pãezinhos recheados no vapor (obtido em todo o processo, da farinha, passando por sovar, abrir a massa, fazer o recheio, rechear e cozinhar no vapor).
	- Ovo frito (obtido em todo o processo, de quebrar o ovo, acender o fogo até virar).
	- Peixe grelhado (obtido grelhando o peixe na fogueira).
	- Objeto indescritível (obtido quando o preparo da comida falha).
	- Carvão (obtido quando o preparo falha por não seguir a receita).

### Comer

- Quando o jogador termina de preparar uma **comida**, pode tentar comê-la.
- Ao comer, o jogador pode tocar na **comida** ou nas **partes da comida** para comê-la.
- Quando o jogador come uma **comida**, há **efeitos sonoros** confortáveis, **textos** reconfortantes e a comida ou as partes dela **desaparecem** com animação para representar a ação de comer.
- Especialmente, quando o jogador come um **objeto indescritível**, há chance de acontecer o seguinte:
	1. O personagem desmaia e acorda depois de um tempo.
	2. O personagem tem um efeito visual de enjoo por um tempo.
	3. Não acontece nada.

---

## ⛺️ Sistema de Acampamento

Só a **barraca** traz sensação de segurança!

### Armazenamento

- Na **barraca**, o jogador pode consultar os **itens** que possui.
- Os itens que o jogador **possui** incluem:
	- Peixes.
	- Colecionáveis.
	- Equipamentos de pesca.
	- Plantações.
- Alguns itens (como alguns colecionáveis) podem ser **expostos**.

### Conquistas

- Na **barraca**, o jogador pode consultar as **conquistas** obtidas.

### Cama

- Ao **pôr do sol** e **à noite**, o jogador pode tocar na cama para **dormir** e pular a noite.
- O jogador acorda no **nascer do sol** ou **pela manhã** do dia seguinte; ele também pode escolher **dormir mais um pouco**.

### Lixeira de reciclagem de emoções

- Essa lixeira, parecida com uma lixeira de reciclagem, permite ao jogador escrever as coisas desagradáveis que aconteceram na **vida real**, amassar tudo numa bolinha e jogar na lixeira de reciclagem de emoções!

### Diário

- O jogador pode escrever no **diário** as coisas que acontecem todos os dias (tanto no jogo quanto na vida real).
- O jogo permite exportar **páginas específicas** do diário para uma **pasta específica** para facilitar o compartilhamento.

### Álbum

- O álbum mostra todas as **obras** que o jogador desenhou no **papel para desenho**.
- O álbum inteiro pode ser exportado como um único arquivo para uma **pasta específica** para facilitar o compartilhamento.

---

## 🐚 Sistema de Comércio

Este melão está maduro?

### Comprar

- O jogador pode comprar produtos no **mercado**.
- No mercado, o jogador pode conversar com **aldeões** de várias profissões.
- Ao **conversar** com os aldeões, há chance de **histórias especiais**; ao concluir essas histórias, os preços podem ser **reduzidos**.
- O jogador pode comprar as seguintes **categorias** de produtos no mercado:
	- Equipamentos de pesca (como varas de pescar).
	- Sementes de plantações (como sementes de trigo).
	- Plantações processadas (como farinha).
	- Vegetais (como acelga chinesa).
	- Combustível (como carvão).
	- Temperos (como sal).
	- Papel para desenho (como papel 1:1).
	- Selos.

### Vender

- O jogador pode vender produtos no **mercado**.
- O jogador pode vender as seguintes **categorias** de produtos no mercado:
	- Peixes.
	- Alguns colecionáveis.
- Ao vender peixes, o **preço do peixe do dia** é a referência.
- O **preço do peixe do dia** se divide em **peixe fresco** e **peixe em estoque**; nenhum dos dois preços é fixo. O preço do dia pode ser determinado em conjunto pelos seguintes fatores:
	- O clima do jogo.
	- A estação do jogo.
	- Um valor aleatório dentro de um intervalo fixo.

### Moeda

- O jogo usa **conchas** como moeda.
- O jogador pode **obter** conchas das seguintes formas:
	- Comerciando.
	- Pesando.
	- Presentes do Cat.

---

## 🌽 Sistema de Cultivos

**Plante**, **regue e adube** e **colha**.

### Plantar

- Para plantar, é preciso ter **sementes**.
- O **processo** de plantio é: afofar o solo, semear, cobrir com terra, regar e adubar.
- As condições para a semente germinar: **umidade adequada**, **temperatura adequada** e **oxigênio suficiente**.
- Ao plantar, o jogador precisa **considerar**:
	- O clima do jogo.
	- A estação do jogo.

### Crescimento

- Durante o crescimento das plantações, o jogador deve manter **a rega** e **a adubação** sem interrupções.
- A cada certo tempo (cerca de 90 horas), a plantação **muda** de **estágio de crescimento**.

### Colheita

- Quando a plantação está **totalmente madura**, o jogador pode colher a **plantação** e as **sementes**.

---

## 🐱 CatGPT

**Converse** com o gatinho ou **faça carinho** nele ฅ՞•ﻌ•՞ฅ.

### Conversar

- O jogador pode **enviar mensagens** para o Cat.
- O Cat **responde** ao jogador com base em certos pesos, que podem ser determinados por:
	1. O número de caracteres enviados pelo jogador.
	2. Uma probabilidade totalmente aleatória.
- O Cat responde com "**Meow**" em vários tons e timbres para dar valor emocional ao jogador.

### Fazer carinho

- O jogador pode tocar suavemente a **cabeça** do Cat para fazer carinho.
- Ao fazer carinho, balões de texto com "**Meow**" voam para fora do Cat, acompanhados de "**Meow**" em vários tons e timbres para dar valor emocional ao jogador.

### Presentes

- O Cat pode dar um **presente** ao jogador quando ele acorda na manhã seguinte.
- Se o Cat dá ou não **presentes** pode ser determinado por:
	1. O número de conversas ou carinhos com o Cat no dia anterior.
	2. O número histórico de conversas ou carinhos com o Cat.
	3. Uma probabilidade totalmente aleatória.
- Os **tipos** de presentes podem incluir:
	- Peixes.
	- Conchas.
	- Alguns colecionáveis (probabilidade mínima).

### Também pode ser...

- Além do Cat, o jogador pode escolher **outros alvos** para conversar ou fazer carinho. Esses **outros alvos** podem ser **membros da equipe de desenvolvimento** que aparecem na **história de introdução**.

---

## 🖌️ Sistema de Desenho

**Desenhe** em papéis e tintas incrivelmente realistas e salve.

### Papel para desenho

- O papel para desenho é igual ao papel real: permite **borrar**, **repintar** e **misturar cores**.
- O jogador pode comprar papel pelo **sistema de comércio**, como papel 1:1 e papel 3:4.

### Paleta de cores

- Por padrão, são oferecidas 8 cores básicas; o jogador pode usar o **pincel** para pegar tinta e misturar na **paleta**.
- O esquema de mistura pode ser **aquarela** ou **guache**.
- Ao misturar, as tintas de duas cores se misturam pelo **pincel**; a tinta não misturada mantém a cor original, e a cor misturada depende do grau de mistura do jogador.

### Pincel

- O pincel pode **aplicar** tinta ou água no papel para desenho.

### Salvar

- As obras desenhadas pelo jogador são **salvas** no **álbum**.
- O jogador pode **exportar** as obras para uma **pasta específica** para facilitar o compartilhamento.

---

## 📬 Sistema de Caixa de Correio

**Receba e envie** mensagens.

### Receber

- O jogador pode **receber** as seguintes mensagens:
	- Cartas que o jogador enviou para si mesmo.
	- Reabastecimento gratuito de iscas.
	- Felicitações de feriados.
	- Felicitações de aniversário.

### Enviar

- O jogador pode **enviar** as seguintes mensagens:
	- Cartas para o eu do futuro.
- Ao enviar, a mensagem deve ter um **selo** colado.

---

## 📺 Interface Visual

**Animações não lineares** fluidas sempre proporcionam uma ótima experiência visual ao jogador.

### Controles

- Os controles podem **acionar** comportamentos de interação e eventos.
- Os controles devem manter o mesmo estilo de design do *Today@PolarBay*.
- Ao **pressionar**, o controle deve encolher instantaneamente e depois voltar com um efeito não linear.
- Os controles podem ter **posição** e **tamanho** personalizados.

### Cartões

- Os cartões não podem ser **interagidos**.
- Os cartões devem manter o mesmo estilo de design do *Today@PolarBay*.
- Os cartões servem para exibir um fundo relativamente **organizado**, como a tela da mochila.

### Tela verde protetora dos olhos

- Como o jogador precisa **fixar os olhos** na **bóia** por **muito tempo** durante a **pesca**, uma **tela verde protetora dos olhos** foi especialmente projetada.
- A tela verde protetora **cobre a tela inteira** de tempos em tempos para **forçar o descanso** do jogador.
- O **intervalo** e a **duração da cobertura** da tela verde protetora podem ser ajustados ou ligados/desligados nas configurações.
- A tela verde protetora exibe o conteúdo das **cartas** das **garrafas à deriva** que o jogador já coletou.

### Esquemas de cores

- O jogo pode ter **dois** esquemas de cores embutidos: o branco e o preto.
- A **troca** entre o branco e o preto pode ocorrer de acordo com:
	1. O dia e a noite da vida real.
	2. O dia e a noite do jogo.
	3. O ajuste manual do jogador na tela de configurações.

### Efeitos de partículas

- Os efeitos de partículas são gerados por **eventos especiais**, como o barco navegando na superfície da água.
- Os efeitos de partículas podem ter a **quantidade** ajustada e podem ser ligados/desligados nas **configurações**, para evitar problemas de desempenho.

### Materiais avançados

- Materiais avançados, ou seja, o material **acrílico**.
- O jogador pode ativar ou desativar os materiais avançados nas **configurações**.
- Com os materiais avançados ativados, as **áreas vazias** dos controles, cartões e outros elementos da interface se tornam um material translúcido e desfocado.

---

## 🕒 Sistema de Tempo

O **tempo** sempre passa tão rápido que perdemos muitas coisas.

### Conversão de tempo

- **Um dia** no jogo equivale a **uma hora** na vida real.
- A proporção de conversão entre o tempo do jogo e o tempo real é **1:24**.

### Faixas horárias

- O **dia** e a **noite** do jogo duram **30 minutos** cada.
- Em **um dia** (60 minutos), as faixas horárias do jogo são divididas assim:
	- Nascer do sol: minutos 1-2.
	- Manhã: minutos 2-10.
	- Meio-dia: minutos 11-20.
	- Tarde: minutos 21-28.
	- Pôr do sol: minutos 29-30.
	- Noite: minutos 31-60.

---

## 💾 Sistema de Salvamento

**Salve** o **progresso atual** do jogo para que nossos peixes e sal fiquem seguros.

### Salvar

- Na página de **salvamento**, o jogador pode tocar no botão **obter save** para **salvar** o progresso atual.
- Na página de **salvamento**, o jogador pode tocar no botão **carregar save** para **carregar** um save salvo.
