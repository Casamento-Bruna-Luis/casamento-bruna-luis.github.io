# 📜 Como Personalizar e Usar a Página do Casamento

## 1. Abrir o arquivo

Abra o arquivo `index.html` em qualquer editor de texto (Bloco de Notas, VS Code, etc.).

---

## 2. Personalizar a Data do Casamento

Localize a linha:
```html
<div class="hero-date fade-in" style="transition-delay: 0.4s;" id="wedding-date">
  ✦ &nbsp; O Grande Dia &nbsp; ✦
</div>
```

Substitua `O Grande Dia` pela data real, por exemplo:
```html
✦ &nbsp; 15 de Novembro de 2025 &nbsp; ✦
```

---

## 3. Inserir a Chave PIX

Localize a linha:
```html
sua-chave-pix@email.com
```

Substitua pelo seu CPF, e-mail, telefone ou chave aleatória PIX real.

---

## 4. Inserir a Foto do Casal

A moldura dourada tem um botão **"Escolher Imagem"** — ao clicar, você pode selecionar
qualquer foto do seu dispositivo. A foto fica salva apenas na sessão atual do navegador.

**Para tornar a foto permanente** (hospedagem), substitua o JavaScript de upload por uma
imagem fixa no HTML:
```html
<!-- Substitua a linha do <img id="couple-photo"> por: -->
<img id="couple-photo" src="foto-casal.jpg" alt="Foto do casal" class="loaded" style="display:block;" />
```
E coloque o arquivo `foto-casal.jpg` na mesma pasta do `index.html`.

---

## 5. Escrever a História de Amor

O campo de texto na seção "Nossa História" é editável diretamente no navegador —
clique e escreva. Para tornar o texto permanente, edite o HTML e substitua o `<textarea>`
por um `<p>` com o texto fixo.

---

## 6. Gerar QR Codes Personalizados para Cada Convidado

A URL da página aceita o parâmetro `?nome=NomeDoConvidado`.

**Exemplos de URLs:**
- `https://seu-site.com/?nome=Ana%20Paula`
- `https://seu-site.com/?nome=Carlos%20e%20Fernanda`
- `https://seu-site.com/?nome=Família%20Silva`

**Para gerar QR Codes gratuitamente:**
1. Acesse [qr-code-generator.com](https://www.qr-code-generator.com/) ou [qrcode-monkey.com](https://www.qrcode-monkey.com/)
2. Cole a URL com o nome do convidado
3. Baixe o QR Code e imprima no convite físico de cada pessoa

---

## 7. Hospedar a Página (para acesso via QR Code)

Para que os convidados possam acessar via QR Code, a página precisa estar hospedada online.

**Opções gratuitas:**
- **Netlify Drop**: arraste a pasta para [app.netlify.com/drop](https://app.netlify.com/drop) — fica online em segundos
- **GitHub Pages**: suba para um repositório GitHub e ative o Pages
- **Vercel**: conecte ao GitHub e faça deploy automático

---

## 8. Estrutura de Arquivos

```
casamento/
├── index.html       ← Página principal (único arquivo necessário)
├── foto-casal.jpg   ← (opcional) Foto fixa do casal
└── COMO_USAR.md     ← Este guia
```

---

*Com amor, bom casamento! 🌹*
