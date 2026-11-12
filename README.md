# Matribox SysCon

Aplicativo independente para controlar e editar a **SONICAKE Matribox II Pro** pelo computador.

Este repositório reúne os downloads, notas de versão e relatos de problemas do SysCon.
O desenvolvimento e a pesquisa do protocolo continuam no [repositório de desenvolvimento](https://github.com/hurricaneabel/matribox-ii-pro-sysex-research).

## Download

**[Baixar a pré-release Windows x64](https://github.com/hurricaneabel/matribox-syscon/releases/tag/v0.1.0-beta.5)**

A primeira distribuição é uma versão portátil leve para testes: não exige instalar
Python ou bibliotecas. O motor de separação de stems por IA não está incluído.

## Como abrir

1. Baixe o ZIP anexado à release e extraia a pasta inteira para um local gravável.
2. Abra **SysCon.exe**. Mantenha a pasta `_internal` junto do executável.
3. Em Configurações, escolha **Oficial** ou **Lab**, conforme o firmware instalado.
4. Feche outros editores que estejam usando a porta MIDI e conecte a pedaleira.

O perfil inicial é Oficial. O aplicativo não instala firmware automaticamente.
Preferências e logs são criados na pasta `userdata`.

## Correção beta.4 — conexão e diagnóstico

Corrigida a recusa de conexão por IDs internos não sequenciais nos presets. O log portátil agora registra erros de sessão tratados. Build 20261108-130121 verificada offline; validação no PC afetado pendente. Mantida a correção visual dos Clones.

Mantida a detecção das portas MIDI da Matribox com numeração variável no Windows, incluindo
`Matribox II Pro Subdevice 3`. Não exige trocar driver nem atualizar firmware.
Baixe e extraia o novo ZIP para usar a correção.

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

## Relatar problemas

Abra uma [issue](https://github.com/hurricaneabel/matribox-syscon/issues), informando Windows, versão do app,
perfil Oficial/Lab, modo Essencial/Pedaleira e os passos para reproduzir.
Quando necessário, anexe `userdata/logs/syscon.log`, revisando o conteúdo antes de publicar.

Projeto independente, sem vínculo oficial com a SONICAKE.
