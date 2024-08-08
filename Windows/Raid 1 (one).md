RAID 1, também conhecido como espelhamento, é uma configuração de arranjo redundante de discos independentes (RAID) que replica os dados em dois ou mais discos. Isso significa que cada dado gravado em um disco é simultaneamente gravado em outro disco, criando uma cópia exata dos dados. Se um dos discos falhar, os dados ainda estarão acessíveis no outro disco, garantindo alta disponibilidade e proteção contra falhas de hardware.

Aqui estão as principais características do RAID 1:

Redundância: Como os dados são espelhados, há uma cópia exata em outro disco, o que garante que, se um disco falhar, os dados não serão perdidos.
Desempenho de leitura: Pode haver uma melhoria no desempenho de leitura, já que os dados podem ser lidos de ambos os discos simultaneamente. No entanto, o desempenho de gravação geralmente não é melhorado, pois os dados precisam ser gravados em ambos os discos.
Capacidade: A capacidade total do RAID 1 é igual ao tamanho do menor disco, pois cada dado é duplicado. Por exemplo, se você usar dois discos de 1 TB em RAID 1, a capacidade utilizável será de 1 TB.
Recuperação de falhas: Em caso de falha de um dos discos, o sistema continua a operar normalmente com o disco restante. Após a substituição do disco com falha, os dados podem ser reconstruídos no novo disco para restaurar a redundância.
RAID 1 é ideal para situações onde a integridade e a disponibilidade dos dados são cruciais, como em servidores de banco de dados ou sistemas de arquivos críticos
