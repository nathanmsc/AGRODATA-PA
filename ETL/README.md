### AGRO DATA

#### IBGE/AGREGADOS

```py
import requests

dados = requests.get(
    "https://servicodados.ibge.gov.br/api/v3/agregados"
).json()

for pesquisa in dados:
    print(f"\n{pesquisa['id']} - {pesquisa['nome']}")
    print(f"Agregados: {len(pesquisa['agregados'])}")
```
```sh

D5 - Áreas Urbanizadas
Agregados: 1

EO - Avaliação dos dados sobre a Biodiversidade Brasileira
Agregados: 3

CL - Cadastro Central de Empresas
Agregados: 27

CA - Censo Agropecuário
Agregados: 1407

ME - Censo Comum do Mercosul, Bolívia e Chile
Agregados: 26

CD - Censo Demográfico
Agregados: 1394

CM - Contagem da População
Agregados: 21

DU - Contas de ecossistemas: o uso da terra nos biomas brasileiros
Agregados: 2

DT - Contas de Espécies Ameaçadas
Agregados: 2

C4 - Contas Econômicas Ambientais da Água
Agregados: 14

DR - Contas Econômicas Ambientais da Terra: Contabilidade Física
Agregados: 1

DZ - Contas Econômicas Ambientais de Energia: produtos da biomassa
Agregados: 12

SU - Contas Nacionais Anuais
Agregados: 1

ST - Contas Nacionais Trimestrais
Agregados: 10

EL - Contribuição dos Polinizadores para as Produções Agrícola e Extrativista do Brasil
Agregados: 1

DE - Demografia das Empresas e Estatísticas de Empreendedorismo
Agregados: 20

D9 - Estatísticas dos Cadastros de Microempreendedores Individuais
Agregados: 10

XF - Estimativas de População
Agregados: 1

FP - Fundações Privadas e Associações Sem Fins Lucrativos
Agregados: 22

IU - Indicadores de Desenvolvimento Sustentável
Agregados: 213

IL - Índice de Preços ao Consumidor em Real
Agregados: 2

IR - Índice de Preços ao Produtor
Agregados: 6

IJ - Índice de Reajuste do Salário Mínimo
Agregados: 2

PC - Índice Nacional de Preços ao Consumidor
Agregados: 13

IA - Índice Nacional de Preços ao Consumidor Amplo
Agregados: 24

IQ - Índice Nacional de Preços ao Consumidor Amplo 15
Agregados: 5

IG - Índice Nacional de Preços ao Consumidor Amplo Especial
Agregados: 8

PG - Índice Nacional de Preços ao Consumidor Especial
Agregados: 2

LA - Levantamento Sistemático da Produção Agrícola
Agregados: 5

C2 - Objetivos de Desenvolvimento Sustentável
Agregados: 234

AC - Pesquisa Anual da Indústria da Construção
Agregados: 59

PB - Pesquisa Anual de Comércio
Agregados: 82

PY - Pesquisa Anual de Serviços
Agregados: 302

PP - Pesquisa da Pecuária Municipal
Agregados: 6

AM - Pesquisa de Assistência Médico-Sanitária
Agregados: 3

ES - Pesquisa de Estoques
Agregados: 9

PM - Pesquisa de Informações Básicas Municipais
Agregados: 187

IT - Pesquisa de Inovação
Agregados: 58

OF - Pesquisa de Orçamentos Familiares
Agregados: 154

SH - Pesquisa de Serviços de Hospedagem
Agregados: 16

SE - Pesquisa de Serviços de Publicidade e Promoção
Agregados: 5

PT - Pesquisa de Serviços de Tecnologia da Informação
Agregados: 5

RC - Pesquisa Estatísticas do Registro Civil
Agregados: 127

PI - Pesquisa Industrial Anual
Agregados: 2

PK - Pesquisa Industrial Anual - Empresa
Agregados: 51

PJ - Pesquisa Industrial Anual - Produto
Agregados: 18

DG - Pesquisa Industrial Mensal - Dados Gerais
Agregados: 32

PZ - Pesquisa Industrial Mensal - Produção Física
Agregados: 26

XY - Pesquisa Industrial Mensal de Emprego e Salário
Agregados: 2

AB - Pesquisa Mensal de Abate de Animais
Agregados: 10

MC - Pesquisa Mensal de Comércio
Agregados: 45

PE - Pesquisa Mensal de Emprego
Agregados: 72

SC - Pesquisa Mensal de Serviços
Agregados: 19

PL - Pesquisa Mensal do Leite
Agregados: 6

SB - Pesquisa Nacional de Saneamento Básico
Agregados: 263

XN - Pesquisa Nacional de Saúde
Agregados: 2222

AA - Pesquisa Nacional de Saúde do Escolar
Agregados: 382

PD - Pesquisa Nacional por Amostra de Domicílios
Agregados: 450

B5 - Pesquisa Nacional por Amostra de Domicílios Contínua anual
Agregados: 1037

BB - Pesquisa Nacional por Amostra de Domicílios Contínua mensal
Agregados: 25

DD - Pesquisa Nacional por Amostra de Domicílios Contínua trimestral
Agregados: 66

AX - Pesquisa Trimestral do Abate de Animais
Agregados: 6

CQ - Pesquisa Trimestral do Couro
Agregados: 5

LT - Pesquisa Trimestral do Leite
Agregados: 3

PA - Produção Agrícola Municipal
Agregados: 7

VS - Produção da Extração Vegetal e da Silvicultura
Agregados: 5

PO - Produção de Ovos de Galinha
Agregados: 4

IO - Produto Interno Bruto dos Municípios
Agregados: 4

XE - Projeção da População
Agregados: 5

SI - Sistema Nacional de Pesquisa de Custos e Índices da Construção Civil
Agregados: 9
```
