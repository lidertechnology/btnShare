# shared-button-component
Componente para compartir sitio web en Angular.


<img width="739" height="468" alt="Captura de pantalla 2025-11-10 a la(s) 3 42 02 p m" src="https://github.com/user-attachments/assets/6970b1df-5c4a-4006-8f54-914677204639" />


# Explicacion del metodo copyToClipboard:

    async copyToClipboard(text: string) {
        try {
          // Intenta copiar el texto al portapapeles usando la Clipboard API
          await navigator.clipboard.writeText(text);
          
          console.log('Texto copiado al portapapeles!'); // Mensaje en la consola si se copia con éxito
        } catch (err) {
          // Si hay un error al copiar, lo muestra en la consola
          console.error('Error al copiar: ', err);
        }
      }
