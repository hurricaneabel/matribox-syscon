# Matribox SysCon

Aplicativo independente para controlar e editar a **SONICAKE Matribox II Pro** pelo computador.

Este repositório reúne os downloads, notas de versão e relatos de problemas do SysCon.

## Download

**[Baixar a pré-release Windows x64 (v0.1.0-beta.6)](https://github.com/hurricaneabel/matribox-syscon/releases/tag/v0.1.0-beta.6)**

Versão portátil para testes: não exige instalar Python ou bibliotecas.
O motor de separação de stems por IA não está incluído.

## Como abrir

1. Baixe o ZIP anexado à release e extraia a pasta inteira para um local gravável.
2. Abra **SysCon.exe**. Mantenha a pasta `_internal` junto do executável.
3. Em Configurações, escolha **Oficial** ou **Lab**, conforme o firmware instalado.
4. Feche outros editores que estejam usando a porta MIDI (incluindo o editor oficial
   da Sonicake) e conecte a pedaleira.

O perfil inicial é Oficial. O aplicativo não instala firmware automaticamente.
Preferências e logs são criados na pasta `userdata`.

## Novidades da beta.6

- O pacote passa a incluir o contrato de licença de uso (`LICENSE.txt`) e os avisos
  dos componentes de terceiros (`THIRD_PARTY_NOTICES.txt`).
- Miniaturas da biblioteca para os Clones 11–20.
- Mantidas as correções anteriores: detecção das portas MIDI com numeração variável no
  Windows, conexão com IDs internos não sequenciais nos presets e correção visual dos Clones.

As versões anteriores (beta.1 a beta.5) não estão mais disponíveis para download.
Baixe e extraia o novo ZIP; não é preciso trocar driver nem atualizar firmware.

## Recursos desta pré-release

- Interfaces **Essencial** e **Pedaleira**, com artes e controles dos efeitos.
- Leitura, edição e gerenciamento de presets; importação NAM/IR e renomeação de slots.
- Perfil Oficial para o firmware padrão.
- Perfil Lab com os recursos compatíveis do firmware modificado: cenas A/B/C,
  volume por cena, comparação de cenas, `.labprst`, CTRL 5/6, E/F, microfones e Hammy Momentary.
- Importação para até 20 Clones no perfil Lab, com firmware compatível.

As funções Lab dependem do firmware correspondente na pedaleira. Selecionar o perfil
não adiciona essas funções ao firmware original. Este download contém somente o app.

## Estado dos testes

Esta é uma **pré-release**, destinada à validação com usuários. A build passou em
autotestes offline dos dois perfis, abertura dos dois modos de interface, backend
MIDI carregado, compilação do conversor NAM e helpers de IR. Esses testes não
comprovam conexão física ou funcionamento em todas as instalações do Windows.

O ZIP tem aproximadamente 2,1 GB, principalmente pelas artes originais dos efeitos.

## Licença

O SysCon é gratuito, mas não é software livre: o uso é regido pelo `LICENSE.txt`
incluído no ZIP (uso pessoal; sem redistribuição, modificação ou engenharia reversa).
Os componentes de terceiros seguem as próprias licenças, listadas em
`THIRD_PARTY_NOTICES.txt` e na pasta `licenses`.

## Relatar problemas

Abra uma [issue](https://github.com/hurricaneabel/matribox-syscon/issues), informando Windows, versão do app,
perfil Oficial/Lab, modo Essencial/Pedaleira e os passos para reproduzir.
Quando necessário, anexe `userdata/logs/syscon.log`, revisando o conteúdo antes de publicar.

Projeto independente, sem vínculo oficial com a SONICAKE.
