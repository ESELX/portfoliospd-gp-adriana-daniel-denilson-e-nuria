---
title: Nome da Máquina
icon: lucide/cog
tags: galeria
status: not-started
hero_image: attachments/Capa.jpg
hero_title: Bambu Lab A1 mini
hero_subtitle: Tutorial detalhado
hero_height: 70vh
hero_overlay: 0.3
hero_align: center
published: true
machine_name: ""
---

# Bambu Lab A1 mini

> A Bambu Lab A1 mini é uma impressora 3D de mesa compacta que serve para fabricar objetos físicos a partir de modelos digitais, sendo usada em prototipagem, design, educação e produção de pequenas peças em contextos domésticos, escolares e profissionais leves.

![](attachments/P1180892.jpg)

Tutorial elaborado pelo grupo seguindo a estrutura de referência (ver tutorial CNC do Fablab Benfica como modelo: <https://fablabbenfica.gitlab.io/fablabbenficadocs/machines/ouplan/>).

## 1. Como desenhar para esta tecnologia?

**Softwares Recomendados**
**Fusion 360 (Autodesk)**  - Modelação paramétrica profissional. Gratuito para estudantes. Ideal para peças mecânicas e funcionais.

**Blender** - Modelação orgânica e artística. Gratuito e open-source. Curva de aprendizagem mais acentuada.

**SolidWorks** - Software profissional de CAD. Disponível em muitas escolas de engenharia.

**OpenSCAD** - Modelação por código (scripting). Excelente para geometrias paramétricas e repetitivas.

==**Boas Práticas para a Modelação:**==

**Geometria fechada (manifold)** - O modelo deve ser completamente fechado, sem faces abertas ou sobrepostas. Usar a ferramenta 'Repair' do Bambu Studio se necessário.
 
 **Orientar o modelo correctamente** - Pensar antecipadamente na orientação de impressão: as superfícies planas ficam melhor apoiadas na base

**Tolerâncias e encaixes** - Para peças que encaixam, adicionar uma folga de 0.2 mm a 0.3 mm entre superfícies.

## 2. Como preparar um ficheiro para a máquina

**Instalação do Bambu Studio**
Descarregar em bambulab.com/download. Disponível para Windows, macOS e Linux. Criar uma conta Bambu gratuita.

1) **Importar o modelo**  - Arrastar o ficheiro .STL/.3MF para a janela, ou File → Import. O modelo aparece na base de impressão virtual.

2)  **Selecionar a impressora** -  No painel direito, confirmar o modelo da Bambu Lab disponível (ex: X1 Carbon, P1S, A1 Mini). Cada impressora tem perfis optimizados.

3)  **Escolher o filamento** - Seleccionar o material (PLA, PETG, ABS, TPU…) e a cor. O Studio ajusta automaticamente temperatura e velocidade

4) **Configurar suportes** - Ativar suportes se o modelo tiver overhang superior a 45°. O tipo 'Tree Support' é mais fácil de remover. Ajustar o ângulo de threshold. 

5) **Fatiar (Slice)** - Clicar em Slice. Verificar a pré-visualização camada a camada para detectar problemas. Verificar estimativa de tempo e material.

6) **Exportar ou enviar** - Exportar como .gcode para cartão SD, ou enviar diretamente para a impressora via Wi-Fi (modo LAN ou conta Bambu Cloud). 

## 3. Antes de Começar

### 3.1. Segurança

**Luvas de proteção** - Para manusear a cama aquecida após impressão ou remover suportes com ferramentas.

**Óculos de segurança** - Ao remover suportes ou fazer pós-processamento (lixar, cortar).

**Máscara FFP2** - Recomendada ao trabalhar com ABS, ASA ou resinas. Também para lixar peças.
### 3.2. Que tipo de ficheiros vou usar e onde os posso produzir

 **.STL** - Formato universal de impressão 3D. Exportado por qualquer CAD. Não preserva escala/cor.

**.OBJ** - Comum em modelação artística (Blender). Aceite pelo Bambu Studio.

**.STEP / .STP -** Para modelação paramétrica. Importável em CAD, converter para STL antes de fatiar
## 4. Como operar a máquina passo-a-passo

Sequência operacional, com fotografias e/ou pequenos vídeos em cada passo crítico.
##### 1. Passo 1 
**Verificar a cama de impressão** 
Confirmar que a superfície de impressão está limpa, sem resíduos de plástico. Limpar com álcool isopropílico 90%+ se necessário. Usar a chapa magnética adequada ao material.
![](attachments/P1180896.jpg)
##### 2. Passo 2
**Verificar o filamento** 
Confirmar que há filamento carregado e que é o material correcto. Verificar que não há humidade (filamento húmido causa bolhas e má adesão).
##### 4. Passo 4
**Via Wi-Fi (Bambu Studio / App)** 
Com a impressora na mesma rede: no Bambu Studio, clicar em 'Send' após fatiar. Escolher a impressora na lista. Confirmar no ecrã da impressora se solicitado.
##### 5. Passo 5
**Via MicroSD / SD** 
Copiar o ficheiro .gcode para o cartão microSD. Inserir na impressora. 
Navegar: Ficheiros → SD Card → seleccionar o ficheiro → Print.
![](attachments/P1180889.jpg)
##### 6. Passo 6
**Monitorizar a impressão** 
Verificar periodicamente. A câmara integrada (modelos X1/P1) permite monitorização remota via app Bambu Handy.
#### Remover a Peça
![](attachments/P1180973.jpg)

1) **Aguardar o arrefecimento** 
   Esperar que a cama arrefeça abaixo de 40 °C (indicado no ecrã). A maioria dos materiais soltam-se espontaneamente com o arrefecimento.

2) **Retirar a chapa magnética** 
   Remover a chapa da cama e flectir ligeiramente a peça soltará sozinha. NUNCA forçar com ferramentas metálicas directamente na superfície de impressão.

3) **Verificar a peça** 
   Inspecionar visualmente: aderência das camadas, qualidade de superfície, deformações (warping), stringing (fios de plástico).
## 5. Resultado e pós-produção

**Acabamentos no objeto impresso** 

**Advertência: Utilizar sempre máscara respiratória e luvas ao utilizar as lixas e primer/tinta de spray!**

1) **Retirar suportes**
   É necessário remover os suportes com cuidado, certificando que não danifique o objeto.

2) **Preparar a superfície**
   Utilizar uma lixa grossa d'água (grão 200 - 400) para remover as marcas dos suportes e as linhas de impressão, com movimentos circulares. Evitar lixar cantos e detalhes pequenos.
   Lixar a seco é possível mas há o risco de derreter o material se este for PLA. Utilizar lixas finas (grão 600 - 1000) para superfícies mais pequenas e para suavizar a superfície do objeto.

3) **Limpeza**
   Quando estiver pronta, utilizar uma escova e àgua para remover o pó deixado pelas lixas ou que tenha ficado preso. Deixar secar completamente.

4) **Aplicar primer(spray)**
   Aplicar entre 2 a 4 camadas de primer spray a uma distância de 15 - 20 cm e rápidamente para evitar acúmulos na superfície. Deixar secar completamente entre as demãos. Este passo é crucial para que a tinta seja uniforme e adira ao plástico.

5) **Finalização**
   Inspecionar o objeto por qualquer imperfeição antes de avançar para a pintura. Caso necessário, utilizar uma lixa de grão 1000 para lixar levemente o primer.

6) **Pintura**
   Podem ser utilizadas ambas tinta em spray ou aerógrafo ou tinta acrílica.
   **Spray** - Borrifar a cor em movimentos constantes e camadas finas a 20 cm da peça para a tinta não escorrer. Se houver várias cores, deixar a core base secar 24 horas antes de prosseguir. Recorrer a fita crepe para cobrir as àreas que não serão pintadas e aplicar a segunda cor. Remover a fita enquanto a tinta ainda está húmida para evitar que esta descasque as bordas. Deixar secar e repetir quantas vezes necessário.
   **Acrílica** - Utilizar pincéis macios e diluír sempre a tinta numa gota de àgua. Aplicar as cores em várias camadas e esperar 10 - 15 minutos entre elas. Para detalhar a pintura, utilizar o método de pincel seco (sujar com tinta e limpar quase tudo com uma tolha de papel, aplicar textura e relevos) ou tinta muito diluida em àgua (para que escorra pela peça para as fendas da impressão e dê um sombreado natural).

7) **Selamento**
    Quando terminar a pintura, utilizar verniz em spray ou verniz acílico para selar a tinta. Dependendo do verniz, pode dar um acabamento fosco, acetinado ou brilhante.
## 6. Recursos e Ficheiros

##### Softwares: 

<p>Bambu Studio →  bambulab.com/download/studio</p>
<p> Bambu Handy (app móvel) → App Store / Google Play → 'Bambu Handy'</p>
<p> Tinkercad →  tinkercad.com</p>
<p>Fusion 360 (estudantes) →   autodesk.com/education/edu-software/overview</p>
<p>Blender  → blender.org/download </p>
<p>PrusaSlicer (alternativa) → prusaslicer.net </p>

##### Repositórios de Modelos 3D

<p>MakerWorld (Bambu) → makerworld.com</p>
<p> Printables→  (Prusa) printables.com </p>
<p>Thingiverse →   thingiverse.com </p>
<p>Cults3D→ cults3d.com </p>
<p> GrabCAD → grabcad.com </p>
<p>MyMiniFactory →  myminifactory.com</p>
