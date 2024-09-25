# unfollowallbluesky

USE POR SUA CONTA E RISCO


Como deixar de seguir todos seus seguidores no bluesky de uma vez.

1. Abra a página de seguidores em um navegador, de preferencia google chrome.

https://bsky.app/profile/username.bsky.social/followers

2. Role a página para baixo o máximo que puder para garantir que o maior número possível de botões 'deixar de seguir' seja exibido.

3. Pressione Ctrl+Shift+I para abrir o console do navegador e digite Permitir Colar.

4. Cole o codigo abaixo em JavaScript que percorre os botões de 'deixar de seguir' e clique em todos eles automaticamente.

"
const buttons = document.querySelectorAll('button');

// Loop through the buttons
buttons.forEach(button => {
    // If button contains the text "Unfollow", click it.
    const buttonText = button.innerText || button.textContent;
    if (buttonText.trim() === 'Unfollow') {
        button.click();
    }
});

"
