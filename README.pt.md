# a11y.co.mz – Acessibilidade da web em Moçambique.
 
# Visão geral
Em dezembro de 2020, o Fórum das Associações Moçambicanas de Pessoas com Deficiência (FAMOD) juntou-se à organização sem fins lucrativos Data4Change, sediada no Reino Unido, para realizar uma investigação baseada em dados sobre a acessibilidade na web de 90 sites importantes de Moçambique. Os sites foram seleccionados pelo FAMOD e variaram de compras online à sites de notícias, sites de emprego e serviços governamentais, bem como do sector privado. Mais informações sobre a investigação e as barreiras enfrentadas, online,  por pessoas com deficiência podem ser encontradas no site do projecto, www.a11y.co.mz.

# Metodologia
Usamos a API da biblioteca ax-core (https://github.com/dequelabs/axe-core) para realizar testes automatizados de acessibilidade em 18.704 páginas da web em 90 sites moçambicanos, de acordo com as diretrizes WCAG.

Para cada um dos sites, links internos (até links internos de nível 2) foram avaliados usando ax-core. Aqui, “links internos de até nível 2” significa; incluindo 102 links especificados inicialmente (links de nível 0), links encontrados em 102 páginas especificadas inicialmente (links de nível 1) e links encontrados em páginas de nível 1 (links de nível 2).

Complementamos o teste automatizado com um dia de teste manual em uma pequena selecção de sites. Isso confirmou ainda mais as barreiras significativas enfrentadas pelos leitores de tela e usuários daltônicos da Internet.

# Resultados
O teste automatizado capturou 722.053 instâncias de 'violações' de acessibilidade. Cada violação representa uma barreira que impede alguém com deficiência visual, auditiva, física ou cognitiva de se engajar totalmente com a página da web.

- Número total de sites avaliados: 90
- Número total de páginas avaliadas: 18.704
- Número total de violações encontradas: 722.053

# Análise
Tomamos a decisão deliberada de não pontuar, avaliar ou comparar sites entre si, uma vez que o teste automatizado só pode testar alguns erros de acessibilidade e, portanto, não podemos comparar sites de maneira justa. (Por exemplo, se os únicos erros de um site fossem 100 imagens sem textos alternativos, uma ferramenta poderia encontrar todos eles e, portanto, 100% dos problemas. No entanto, se um site tivesse um problema relacionado à ordem de foco, uma ferramenta poderia não encontrar este problema e obteria 0% dos problemas.)

Nossos resultados podem nos dizer as violações de acessibilidade mais comuns encontradas por testes automatizados. As cinco principais violações de acessibilidade foram as seguintes (e representam quase 90% de todas as violações de acessibilidade nas páginas da web que testamos):
- 37% das violações: os elementos têm contraste de cor insuficiente
- 33%: Nem todo o conteúdo da página é composto por pontos de referência (*landmarks*)
- 11%: Os links não têm texto discernível
- 3%: Os elementos de Selecção não têm nomes acessíveis
- 2%: As imagens não possuem texto alternativo

Observação: Ao agregar esta lista, excluímos violações "menores", como “o valor do atributo id deve ser único”. Também combinamos a violação “O documento deve ter um ponto de referência principal” com “Todo o conteúdo da página deve estar contido em pontos de referência” e a violação “Os elementos do formulário devem ter rótulos” com “O elemento de Selecção deve ter um nome acessível".

# Dados
O arquivo **pages.csv** contém os resultados de cada uma das 18.704 páginas testadas, detalhando o número de regras de acessibilidade aprovadas, violadas, inaplicáveis ​​e incompletas por página.

# Dicionário de dados
*lista de cada nome de coluna e sua descrição futura*

# Sobre
## Sobre a11y.co.mz
“A11y” é uma abreviatura comum para “*accessibility*”. O “11” representa o número de letras entre o “a” e “y” na palavra "*accessibility*". a11y.co.mz foi projectado e desenvolvido por Amílcar Carlos Paco (Gerente de TI e Engenheiro de Dados do FAMOD) e Data4Change. O FAMOD está entre as 13 organizações da sociedade civil que tiveram sucesso em se candidatar ao Fundo Africano de Direitos Digitais administrado pela CIPESA (Colaboração sobre Política Internacional de TIC na África Oriental e Austral). O Fundo Africano de Direitos Digitais incluiu a oportunidade de receber treinamento em habilidades de dados e trabalhar em projectos baseados em dados com Data4Change.

## Sobre FAMOD
FAMOD é uma organização que tem como membros as organizações da sociedade civil que trabalham no apoio às pessoas com deficiência em Moçambique. FAMOD foi fundada em 2003 e trabalha para apoiar, coordenar e representar os interesses das suas organizações membros, bem como para promover os direitos humanos e o bem-estar das pessoas com deficiência em Moçambique. FAMOD trabalha actualmente para assegurar que as pessoas com deficiência, incluindo mulheres e crianças, não sejam deixadas para trás nos planos de resposta e recuperação da Covid-19. Visite www.famod.org para mais informações.

## Sobre Data4Change
Data4Change é uma organização sem fins lucrativos sediada no Reino Unido. Eles criam projectos baseados em dados com o objectivo de resolver alguns dos desafios sociais e políticos mais prementes do mundo. Visite www.data4chan.ge para obter mais informações.

## Sobre CIPESA
Este projecto foi realizado no contexto do Fundo de Direitos Digitais da África com o apoio da Colaboração sobre Política Internacional de TIC para a África Oriental e Austral (CIPESA). Desde a sua fundação, a CIPESA posicionou-se como um centro líder para pesquisa e análise de informações destinadas a permitir que os formuladores de políticas na região entendam as questões das políticas de TIC e para que várias partes interessadas usem as TIC para melhorar os meios de subsistência. Visite www.cipesa.org para mais informações.
