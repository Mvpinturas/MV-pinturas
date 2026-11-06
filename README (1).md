# MV Pintura — aplicativo Android

Projeto Android nativo em Kotlin + Jetpack Compose, com banco local Room.

## Recursos incluídos
- Cadastro de clientes (nome, telefone, CPF/CNPJ, endereço e observações).
- Cadastro de orçamentos vinculados ao cliente.
- Descrição do serviço, materiais, mão de obra, materiais e pagamento.
- Histórico com situação: pendente, aprovado ou recusado.
- Painel com indicadores.
- Geração de PDF e compartilhamento pelo menu do Android (incluindo WhatsApp quando instalado).
- Banco de dados local persistente (`mv-pintura.db`).

## Como gerar o APK
1. Instale o Android Studio (versão recente) em um computador.
2. Abra a pasta `MVPinturaAndroid`.
3. Aguarde a sincronização do Gradle.
4. Selecione **Build > Build Bundle(s) / APK(s) > Build APK(s)**.
5. O APK de teste ficará em `app/build/outputs/apk/debug/app-debug.apk`.

## Observações importantes
- Este pacote contém o código-fonte do aplicativo Android. O APK ainda precisa ser compilado no Android Studio; não foi compilado nem instalado neste ambiente.
- Os dados ficam armazenados localmente no aparelho. Para sincronizar entre vários celulares, será necessário adicionar um backend com autenticação e cópias de segurança.
- O botão de compartilhamento abre o menu nativo do Android para escolher WhatsApp ou outro aplicativo. O envio final é confirmado pelo usuário no WhatsApp.
- Valores devem ser digitados em reais usando ponto decimal no campo numérico (ex.: `1200.00`).
- Revise os dados comerciais e o modelo do PDF antes de usar com clientes.
