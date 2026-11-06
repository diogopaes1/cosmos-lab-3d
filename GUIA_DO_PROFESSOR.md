# COSMOS LAB 3D
## Laboratório interativo de astrofísica para o ensino médio

**Versão 1.0 | Projeto escolar | Idioma: português brasileiro**

**Criado por Diogo Paes da Costa (2026)**

Este material foi elaborado para uma atividade didática sobre evolução estelar, gravitação, objetos compactos e núcleos galácticos ativos. O simulador é uma representação ilustrativa com controles interativos, não um modelo astrofísico completo.

## Como executar

1. **No computador:** abra `index.html` em uma versão atual do Chrome, Edge, Firefox ou Safari.
2. **No celular:** abra o arquivo HTML no navegador. Se o aplicativo de arquivos ou de mensagens impedir a execução do HTML, acesse uma versão publicada na web.
3. **Para publicar e compartilhar por link:** carregue `index.html` em um serviço de hospedagem de páginas estáticas, como GitHub Pages. Depois, envie o endereço aos alunos ou gere um QR code desse endereço. O botão de compartilhamento do simulador envia também a configuração atual do experimento pelo próprio link.
4. O simulador funciona sem conexão com a internet depois de aberto como arquivo. **Os links para fontes NASA e DOE**, na barra lateral, requerem conexão.

O projeto não exige cadastro dos estudantes, não usa bibliotecas externas e não envia os parâmetros a servidores. WebGL é o motor 3D preferencial. Caso esteja indisponível, o sistema utiliza uma visualização gráfica alternativa em Canvas.

## Modos de aprendizagem

**Explorar:** selecione estrela, gigante vermelha, anã branca, estrela de nêutrons, buraco negro ou quasar. Ajuste massa, temperatura, rotação ilustrativa, intensidade dos feixes ou gás em acreção, conforme o objeto. Observe o raio e outros indicadores derivados.

**Evolução:** selecione a massa *inicial* da estrela, depois avance o controle de etapas. O destino mostrado é aproximado: abaixo de ~8 massas solares, anã branca; de ~8 a 25, estrela de nêutrons; acima de ~25, buraco negro. Os limites não são exatos e mudam conforme a perda de massa, composição química, rotação e evolução em sistemas binários.

**Colapso:** selecione a massa e comprima o raio. O programa utiliza Rₛ = 2GM/c² para mostrar o raio de Schwarzschild de um corpo idealizado, esférico e sem rotação. Um horizonte de eventos é indicado quando R ≤ Rₛ. O experimento é hipotético e não simula o comportamento real de matéria durante o colapso.

## Proposta de aula de 25 a 35 minutos

1. **5 min | Hipótese:** pergunte se toda estrela termina como um buraco negro e se um quasar é uma estrela.
2. **8 min | Evolução:** os grupos testam as massas iniciais 3, 15 e 40 M☉. Registram o destino de cada uma. Discutam por que os resultados são tendências, e não garantias.
3. **6 min | Estrela de nêutrons:** selecionar o objeto e comparar **Comum**, **Pulsar** e **Magnetar**. Mudar rotação e feixes, e explicar por que um pulsar pode se comportar como um farol.
4. **6 min | Buraco negro e quasar:** comparar ambos; reduzir a acreção do quasar até zero. Em **Mais opções de visualização**, comparar os perfis **Cinema** e **Doppler**, e os ângulos de observação. Discutir por que o buraco negro continua existindo quando a atividade luminosa cessa.
5. **5–10 min | Compressão:** selecionar 1 M☉, reduzir o raio gradualmente e identificar o limite aproximado de 2,95 km. Perguntar por que isso não descreve o destino real do Sol.

## Perguntas para avaliação

1. Qual a diferença entre **massa inicial de uma estrela** e **massa do remanescente**?
2. Como uma estrela de nêutrons pode produzir pulsos periódicos?
3. Um buraco negro sem gás ao redor precisa apresentar um disco brilhante?
4. Um quasar é um novo tipo de estrela ou um núcleo galáctico ativo?
5. No modelo idealizado, o que acontece com o raio de Schwarzschild se a massa de um objeto dobra?

**Respostas esperadas:** (1) uma estrela pode perder grande parte da sua massa antes de formar o remanescente; (2) a rotação varre o espaço com feixes de radiação e só detectamos pulsos conforme a orientação; (3) não; (4) núcleo galáctico ativo; (5) ele dobra.

## Cuidados científicos

- O tamanho aparente dos objetos **não está na mesma escala**. Sem esse recurso, o núcleo de nêutrons seria invisível junto de uma estrela comum.
- O brilho e as cores são representações artísticas; a emissão real de certos objetos ocorre em outras faixas do espectro eletromagnético.
- A animação da rotação não representa a velocidade real.
- As curvas do disco e os anéis luminosos próximos a buracos negros são ilustrativos e **não** resultam de uma integração completa das equações da relatividade geral.
- Um quasar precisa de um buraco negro supermassivo e de gás suficiente para alimentar um núcleo ativo; **não** resulta simplesmente do aumento de massa de uma estrela de nêutrons.
- O valor de luminosidade estelar, quando mostrado, é estimado pela relação L/L☉ ≈ (R/R☉)² (T/5772 K)⁴, usando um raio aproximado do tipo de estrela.
- O raio do horizonte do modo Colapso corresponde ao caso **sem rotação** e sem carga elétrica.

## Fontes de referência

- NASA, Black Holes: https://science.nasa.gov/universe/black-holes/
- NASA, Hubble Pulsars: https://science.nasa.gov/mission/hubble/science/science-behind-the-discoveries/hubble-pulsars/
- NASA, Anatomy of a Black Hole: https://science.nasa.gov/universe/black-holes/anatomy/
- U.S. Department of Energy, How Large Are Neutron Stars?: https://www.energy.gov/science/np/articles/how-large-are-neutron-stars

## Conteúdo do pacote

- `index.html`: simulador interativo, pronto para servir como página inicial de um site.
- `GUIA_DO_PROFESSOR.md`: este documento.
- `PREVIA_*.png`: capturas geradas com o shader WebGL em execução de teste, sem compor a interface real.

**Nota:** para futuras alterações e personalização da marca da escola, o HTML é um arquivo de texto editável, inclusive sem conexão com a internet.

## Comparação orientada entre as imagens do buraco negro

No perfil **Cinema**, a imagem tende a ser mais equilibrada entre os lados. O perfil **Doppler** aumenta qualitativamente o brilho do lado do disco que se move na direção do observador. Compare a estrutura aparente que passa acima e abaixo da sombra, causada pela deflexão gravitacional na representação. **O shader não integra geodésicas relativísticas** e seus perfis não permitem medir parâmetros astrofísicos reais. Os arcos de magnetar representam linhas de campo esquemáticas, não luz visível do campo magnético.

O modo de magnetar enfatiza a intensidade e a configuração do campo. O modo de pulsar enfatiza emissões que podem ser detectadas como pulsos, dependendo da orientação. Magnetar e pulsar não são etapas obrigatórias e sequenciais na vida de toda estrela de nêutrons.