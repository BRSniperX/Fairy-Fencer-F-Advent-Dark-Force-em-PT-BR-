<img width="1672" height="941" alt="1-steam" src="https://github.com/user-attachments/assets/1914139e-af0d-410d-a8d3-d9fb9ff36247" />
# Fairy Fencer F: Advent Dark Force — Tradução PT-BR v1.2

## Novidades da v1.2

- **Tutorial «Wait» traduzido.** A caixa de texto do tutorial (segundo mapa, depois do chefe bandido) estava em
  inglês: a entrada `dbHelp` 105 só existe no banco ocidental (EN/CN) e, como a tradução é casada pelo id do
  japonês, ficou de fora. Uma varredura do texto instalado contra o inglês original achou mais 16 entradas do
  banco na mesma situação (avisos da Caixa de Música, da Caixa de Imagens e do serviço de síntese, duas
  habilidades e o aviso «Ajuda adicional»); todas traduzidas.

## Novidades da v1.1

- **Corrigido o travamento ao subir de nível:** na v1.0 o jogo fechava com erro (ou ficava em tela preta) na tela de status da subida de nível, a partir da primeira. O defeito estava na animação «SUBIU DE NÍVEL!»; agora ela aparece normalmente.

**Já tem a tradução instalada?**
- Da **v1.1**: basta copiar `jogo\ENSystem.bra` deste pacote por cima do da pasta do jogo.
- Da **v1.0**: copie `jogo\ENSystem.bra` e `jogo\ENGame.bra`.

Os outros arquivos não mudaram. Os saves não são afetados.

---


Tradução para português do Brasil de **Fairy Fencer F: Advent Dark Force** (PC / Steam).

Traduz **o jogo inteiro**: todo o texto, as DLCs, as opções de PC, **as imagens** — menus,
placas de batalha, tela de resultado, letreiros — e os **vídeos com texto**.

> ⚠️ **O texto do jogo precisa estar em INGLÊS.** Esta tradução reescreve os arquivos do
> idioma inglês — ela não adiciona um idioma novo. Com o texto em japonês ou chinês, a
> tradução não aparece.

---

## Feita a partir do japonês

A base é o **texto japonês**, não o inglês. O inglês de *Advent Dark Force* reescreve falas e
troca nomes; aqui vale o original:

- Nomes da **localização oficial ocidental** onde ela só localizou (**Fang**, **Eryn**,
  **Tiara**, **Lola**, **Khalara**, **Marianna**) e o **japonês** onde o inglês inventou ou
  trocou sem necessidade: **Mestre** (EN «Guillermo»), **Mitsubo** (EN «Mrs. Five-Star»).
- 魔神, a terceira divindade, não tem gênero no japonês: é a **Divindade Demoníaca**, e não
  «Evil Goddess».
- Onde o inglês errou, o português acerta: três ofertas que o inglês anuncia por `9990 G`
  cobram 9980 no jogo — fica **9980**, como no japonês; e uma fala que tinha ficado em
  coreano no inglês (`3500 Gold를 지불했다`) agora é **«Você pagou 3500 de ouro.»**

**Recomendamos jogar com as vozes em japonês.**

---

## O texto

| | |
|---|---|
| Cenas das três rotas | **15.426 falas**, revisadas duas vezes contra o japonês |
| Menus, itens, armas, habilidades, inimigos, fadas, missões, sinopses, galeria | completos |
| Escolhas e avisos das cenas | completos |
| DLCs (fadas extras, itens, andares ocultos, AMADOR e INFERNO) | completas |
| Opções de PC, salvar/carregar, menu de DLC, remapeamento | via `dinput8.dll`, sem alterar o exe |

Mais de **32 mil entradas** no total. Nomes de habilidades e combos em português, com formas
curtas para a lista de combos.

## As imagens e os vídeos

**197 imagens refeitas**, além das peças de texto dos atlas da interface, com o degradê e o
contorno de cada tela:

- **Batalha** — `Esquiva`, `Defesa Crítica`, `Custo WP`, `Acertos`, `Alcance`, `Efeito extra`,
  `Líder`, `MEMBRO ATIVO`, `Aguardar`.
- **Resultado** — `RESULTADO`, `DANO TOTAL`, `NOVO RECORDE!!`, `EXP Obtido`, `Valor Obtido`,
  `WP Obtido`, `Itens Obtidos`, `MÁX Dano`, `MÁX Combo`.
- **Telas** — título, dificuldades, `CARREGANDO`, `SUBIU DE NÍVEL!`, `EVENTO`, `CAPÍTULO`,
  `CATEGORIA`, `CUMPRIDA`, `Feito!`.
- **Letreiros de tempo** das cenas e faixas da DLC08.
- **Vídeos** — prólogo (cartões em português), letreiro «Cidade de Zelwinds» e o vídeo das
  lembranças (legenda em português, com voz japonesa).

---

## Instalação

1. **Feche o jogo** e faça backup dos arquivos que o pacote substitui (lista em `ARQUIVOS.txt`).
2. Extraia o `.zip` e copie **o conteúdo da pasta `jogo`** para a pasta do jogo, **substituindo**
   os arquivos — normalmente `...\steamapps\common\Fairy Fencer F Advent Dark Force\`. O
   `dinput8.dll` tem de ficar ao lado do `FairyFencerAD.exe`.
3. Da pasta `DLC`, copie **só os `DLC0x.bra` que já existem** na pasta do seu jogo.
4. No jogo, opções de PC → **Text Select** («Idioma do texto») → **English** («Inglês») e
   **reinicie**.

São **23 arquivos** (15 em `jogo`, 8 em `DLC`); o MD5 de cada um está em `ARQUIVOS.txt`.

### O `dinput8.dll`

Alguns textos ficam dentro do executável. **O `FairyFencerAD.exe` não é alterado**: o
`dinput8.dll`, carregado pelo próprio jogo, troca esses textos só na memória (`ptbr_exe.txt`)
e ajusta a ordem de dois rótulos da tela de resultado (`ptbr_patch.txt`). Cada troca só é
aplicada se os bytes originais estiverem lá: com outro executável, não faz nada.

### Não funcionou?

| O que você vê | Causa quase certa |
|---|---|
| Jogo em inglês, sem nada em português | Os arquivos ficaram numa subpasta; eles vão ao lado do `FairyFencerAD.exe` |
| Jogo em japonês ou chinês | O texto não está em inglês; troque em «Text Select» e reinicie |
| Opções de PC e menu de DLC em inglês | `dinput8.dll` e os `.txt` fora do lugar, ou bloqueados pelo antivírus |
| Textos de uma DLC em inglês | O `DLC0x.bra` daquela DLC não foi copiado |
| O português sumiu depois de um tempo | A Steam verificou os arquivos; reinstale |
| O jogo não abre | Apague o `dinput8.dll`; se continuar, restaure o backup e reporte |

Para desinstalar, apague `dinput8.dll`, `ptbr_exe.txt` e `ptbr_patch.txt` e restaure o backup
ou use *Verificar integridade dos arquivos* na Steam.

---

## O que ficou de fora

- **Tutoriais** — ficam como no original.
- **`GAME OVER`**, **`LEVEL UP!!`**, **`STOP`** e **`AUTO`** — mantidos como no original.
- **Logotipos e créditos** dos vídeos.
- **Saves antigos** — missões já aceitas num save anterior à tradução podem manter o título em
  inglês (fica gravado no save). As novas saem em português.
- Imagens comuns a todos os idiomas (título, dificuldades, alguns letreiros) aparecem em
  português mesmo com o texto em japonês ou chinês.

Encontrou algo? Abra uma issue com um print e a tela ou o lugar onde apareceu.

---

*Fairy Fencer F: Advent Dark Force* © IDEA FACTORY / COMPILE HEART. Todos os direitos
reservados. Projeto de fã, gratuito e sem fins lucrativos, sem vínculo com a Idea Factory, a
Compile Heart ou a Idea Factory International.
