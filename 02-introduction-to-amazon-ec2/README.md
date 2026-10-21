# ☁️ Introduction to Amazon EC2

Laboratório prático realizado durante meus estudos de Computação em Nuvem, com foco na criação, configuração, monitoramento e gerenciamento de uma instância Amazon EC2.

## 🎯 Objetivo

Praticar conceitos fundamentais da AWS por meio da implantação de um servidor web, configuração de rede e segurança, monitoramento de recursos e gerenciamento do ciclo de vida de uma instância EC2.

## 🛠️ Tecnologias e serviços utilizados

- **Amazon EC2:** criação e gerenciamento de servidor virtual.
- **Amazon Linux 2023:** sistema operacional da instância.
- **Amazon EBS:** armazenamento em bloco.
- **Security Groups:** controle do tráfego de rede.
- **Amazon CloudWatch:** visualização de métricas de monitoramento.
- **Apache HTTP Server (`httpd`):** servidor web instalado por meio de User Data.
- **User Data:** execução automatizada de comandos durante a inicialização.

## 🔧 Atividades realizadas

### 1. Criação e configuração da instância

- Criação de uma instância EC2 com o nome `Web Server`.
- Seleção da AMI Amazon Linux 2023 e do tipo `t3.micro`.
- Configuração da rede e do grupo de segurança.
- Ativação da proteção contra encerramento.
- Configuração de um script de inicialização para instalar e iniciar o Apache.

### 2. Monitoramento

- Verificação do estado da instância e das verificações de integridade.
- Consulta às métricas disponíveis na guia Monitoring.
- Exploração do recurso de captura de tela da instância para apoio à análise e solução de problemas.

### 3. Configuração de acesso HTTP

Inicialmente, o servidor não estava acessível pelo navegador porque o grupo de segurança não permitia tráfego HTTP de entrada.

Para corrigir o problema, adicionei uma regra de entrada permitindo HTTP pela porta 80 e testei novamente o acesso ao servidor.

**Ponto prático de troubleshooting:** durante o teste, precisei ajustar manualmente o protocolo no endereço do navegador, alterando `https://` para `http://`, para visualizar a página do servidor.

Após os ajustes, consegui visualizar a mensagem:

`Hello From Your Web Server!`

### 4. Redimensionamento de recursos

- Interrupção da instância antes da alteração.
- Mudança do tipo de instância de `t3.micro` para `t3.small`.
- Aumento do volume EBS de 8 GiB para 10 GiB.
- Reinicialização da instância após as modificações.

### 5. Proteção contra encerramento e finalização

- Teste da proteção contra encerramento da instância.
- Verificação de que a proteção impedia a exclusão enquanto estivesse habilitada.
- Desativação da proteção para permitir o encerramento.
- Finalização da instância ao concluir as atividades.

## 💡 Principais aprendizados

- Compreensão do ciclo de vida de uma instância EC2.
- Noções práticas de configuração de recursos computacionais na nuvem.
- Uso de User Data para automatizar tarefas de inicialização.
- Entendimento da função dos Security Groups no controle de acesso.
- Identificação de possíveis causas de falha no acesso a um servidor web.
- Noções de monitoramento, escalabilidade vertical e armazenamento EBS.
- Importância de validar as configurações e testar o resultado após cada alteração.

## 🧩 Troubleshooting na prática

Durante a validação do servidor web, foi necessário corrigir o protocolo utilizado na URL do navegador de HTTPS para HTTP.

Esse ajuste reforçou a importância de verificar o protocolo de comunicação esperado pelo serviço, além das configurações de rede e das regras de acesso.

## ✅ Resultado

Laboratório concluído dentro do tempo disponibilizado, seguindo as instruções propostas e validando o funcionamento do servidor web no navegador.

Este exercício faz parte do meu processo de desenvolvimento de habilidades práticas em Linux, Redes, AWS e Cloud Computing, com foco em Suporte Técnico e Cloud Support.

---

*Documentação elaborada a partir da minha execução prática do laboratório.*