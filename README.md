# Cosmos Lab 3D

**Laboratório interativo de astrofísica para o ensino médio**  
**Criado por Diogo Paes da Costa (2026) · V 1.0**

## Abrir

Abra `index.html` no Chrome, Edge, Safari ou Firefox. O programa reúne HTML, CSS, JavaScript e o shader WebGL no mesmo arquivo. Não precisa de instalação nem de conexão de rede para a atividade local.

## Novidades visuais

- Disco de acreção com arcos aparentes acima e abaixo do buraco negro, ilustrando o desvio da luz.
- Comparação entre tratamento **Cinema** (brilho aproximadamente simétrico) e **Doppler** (assimetria qualitativa de brilho).
- Controle do ângulo de observação na seção opcional **Mais opções de visualização**.
- Estrela de nêutrons em cenários **Comum**, **Pulsar** e **Magnetar**.
- Jatos do quasar que podem ser exibidos ou ocultados.
- Visualização alternativa Canvas 2D em dispositivos sem WebGL.

## Aviso científico

Este é um **modelo educacional ilustrativo**, não um simulador numérico relativístico. A curvatura luminosa, os jatos, a aparência das superfícies e o brilho são aproximações gráficas. O modelo de colapso aplica o raio de Schwarzschild apenas ao caso idealizado sem rotação e sem carga; a evolução estelar utiliza faixas aproximadas de massa inicial. Os corpos estão fora de escala entre si.

## Publicar de forma independente

Escolha um **repositório exclusivo**, por exemplo `cosmos-lab-3d`, ou uma hospedagem estática própria. **Não** coloque o Cosmos Lab em pastas do projeto MOS UFAPE.

### GitHub Pages

1. Crie um repositório público `cosmos-lab-3d` separado de outros projetos.
2. Coloque `index.html` na raiz da branch principal.
3. Em **Settings → Pages → Build and deployment → Deploy from a branch**, selecione a branch `main` e a pasta `/(root)`.
4. Acesse o endereço real exibido na seção Pages após a publicação. Para a conta `diogopaes1`, o formato esperado do endereço é `https://diogopaes1.github.io/cosmos-lab-3d/`. Verifique que a página existe antes de distribuir o link.

### Netlify Drop

Alternativamente, abra https://app.netlify.com/drop e arraste **a pasta com `index.html`** para a área de publicação. O endereço final será fornecido pelo serviço. Para manter o site e atualizar novas versões, faça login e vincule o projeto à sua conta.

## Conteúdo deste pacote

- `index.html` — aplicação completa
- `GUIA_DO_PROFESSOR.md` — explicação da atividade e limitações
- `README.md` — instruções de uso e publicação
- `PREVIA_*.png` — capturas dos modelos 3D testados (ilustrativas)