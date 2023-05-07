import github
from github import Github

# Autentique-se usando uma token de acesso pessoal ou as credenciais do GitHub
g = Github("sua_token_de_acesso_pessoal_aqui")

# Acesse informações do usuário conectado
user = g.get_user()
print("Nome do usuário:", user.name)
print("Avatar do usuário:", user.avatar_url)
print("Número de repositórios públicos:", user.public_repos)
