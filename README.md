[README.md](https://github.com/user-attachments/files/23413308/README.md)
# Ferramentaria Inteligente - Correção de Câmera

Esta versão contém correções para o problema de inicialização da **câmera traseira** em tablets.

## 🧩 Alterações principais

- Substituição das funções `startGlobalScanner` e `startToolScanner` para seleção automática da câmera traseira (`back`, `rear`, `environment`).
- Adição de logs de depuração (`console.log`) para ajudar a identificar qual câmera foi selecionada.
- Tratamento aprimorado de erros com mensagens de orientação ao usuário.
- Compatibilidade garantida com Chrome, Edge, Safari e WebViews que implementam corretamente o `getUserMedia`.

## 🚀 Como testar

1. Hospede o arquivo em um servidor **HTTPS** ou use `localhost`.
2. Abra o app em um **tablet Android** ou **iPad** e **permita o acesso à câmera**.
3. Se aparecer `Permissão negada`, verifique:
   - As permissões do navegador (Configurações → Apps → [Navegador] → Permissões → Câmera).
   - Se o dispositivo está em HTTPS.
4. O console (F12 → Console) mostrará qual câmera foi detectada e selecionada.

## 🛠 Estrutura do pacote

```
ferramentaria_app_camera_fix.zip
├── index_updated.html   # HTML principal com correção de câmera
└── README.md            # Instruções e notas de versão
```

## 📄 Licença

Distribuição livre para uso interno e testes corporativos.
