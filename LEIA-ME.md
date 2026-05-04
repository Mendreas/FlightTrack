# Flight Track Viewer — App Desktop

## Pré-requisitos

Instala o **Node.js** (versão 18 ou superior):
👉 https://nodejs.org/en/download

Escolhe "Windows Installer (.msi)" e instala com as opções por defeito.

---

## Passos para instalar e testar

### 1. Abre uma janela de Terminal (Command Prompt ou PowerShell)

No Windows: Prima `Win + R`, escreve `cmd`, clica OK.

### 2. Navega até à pasta do projeto

```
cd C:\caminho\para\flight-tracker-electron
```
(substitui pelo caminho onde colocaste esta pasta)

### 3. Instala as dependências

```
npm install
```

Aguarda. Vai descarregar o Electron e o electron-builder (~200 MB).

### 4. Testa a app

```
npm start
```

A janela da app deve abrir. Se funcionar bem, podes avançar para criar o instalador.

---

## Criar instalador (.exe para Windows)

```
npm run dist-win
```

O ficheiro instalador aparece na pasta `dist/` com o nome `Flight Track Viewer Setup x.x.x.exe`.

Basta fazer duplo clique para instalar. A app aparece no menu Iniciar.

---

## Notas importantes

- A app **precisa de internet** para carregar os mapas (tiles CartoDB).
- O ficheiro `index.html` é a tua app original — podes substituí-lo por versões actualizadas quando quiseres.
- Para Mac: usa `npm run dist-mac` numa máquina macOS.
- Para Linux: usa `npm run dist-linux`.
