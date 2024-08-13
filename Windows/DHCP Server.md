O DHCP (Dynamic Host Configuration Protocol) é um serviço de rede que permite que os dispositivos na rede obtenham automaticamente endereços IP e outras configurações de rede, como máscara de sub-rede, gateway padrão e servidores DNS. No Windows Server, você pode configurar o DHCP para distribuir essas informações automaticamente para dispositivos clientes na rede.

Passos para configurar o DHCP no Windows Server:
Instalar o Serviço DHCP:

Abra o "Gerenciador de Servidores" (Server Manager).
Clique em "Adicionar funções e recursos" (Add roles and features).
No assistente, selecione "Instalação baseada em funções ou recursos" (Role-based or feature-based installation).
Selecione o servidor em que você deseja instalar o DHCP e clique em "Avançar".
Na lista de funções, marque a caixa "Servidor DHCP" (DHCP Server) e clique em "Avançar".
Continue com o assistente até a instalação ser concluída.
Configurar o Servidor DHCP:

Após a instalação, abra o "DHCP" a partir do "Gerenciador de Servidores" (Server Manager) ou do "Painel de Controle".
Expanda o nome do servidor na árvore de console e clique com o botão direito em "IPv4" e selecione "Nova Escopo..." (New Scope...).
Siga o assistente para criar um novo escopo. Você precisará definir:
Nome do escopo.
Intervalo de endereços IP a serem distribuídos.
Máscara de sub-rede.
Configurações adicionais como gateway padrão (roteador), servidores DNS, e WINS (se necessário).
Após concluir o assistente, ative o escopo.
Configurar Opções Adicionais do DHCP (Opcional):

No DHCP, você pode configurar opções adicionais, como:
Reservas: Permitir que certos dispositivos sempre recebam o mesmo endereço IP.
Exclusões: Definir IPs que não devem ser distribuídos.
Opções de escopo: Configurações como o tempo de lease (aluguel do IP), opções de roteador, etc.
Autorizar o Servidor DHCP:

Em "Gerenciador de Servidores" (Server Manager), verifique se o servidor DHCP está autorizado no Active Directory.
Clique com o botão direito no servidor DHCP no console DHCP e selecione "Autorizar" (Authorize).
Verificação e Testes:
Para testar se o DHCP está funcionando, conecte um dispositivo à rede e configure-o para obter um endereço IP automaticamente. Verifique se ele recebe um IP do intervalo configurado.
