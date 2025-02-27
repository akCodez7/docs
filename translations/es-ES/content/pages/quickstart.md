---
title: Guía de inicio rápido para GitHub Pages
intro: 'Puedes utilizar {% data variables.product.prodname_pages %} para mostrar algunos proyectos de código abierto, hospedar un blog o incluso compartir tu CV. Esta guía te ayudará a iniciar creando tu siguiente sitio web.'
allowTitleToDifferFromFilename: true
versions:
  fpt: '*'
  ghes: '*'
  ghae: '*'
  ghec: '*'
type: quick_start
topics:
  - Pages
shortTitle: Inicio Rápido
product: '{% data reusables.gated-features.pages %}'
---

## Introducción

Las {% data variables.product.prodname_pages %} son páginas web públicas que se publican a través de {% data variables.product.product_name %}. La forma más rápida de iniciar es utilizando el Selector de Temas de Jekyll para que cargue un tema preconfigurado. Posteriormente, podrás modificar el estilo y contenido de tus {% data variables.product.prodname_pages %}.

Esta guía te mostrará cómo crear un sitio de usuario en `username.github.io`.

## Crear tu sitio web

{% data reusables.repositories.create_new %}
1. Enter `username.github.io` as the repository name. Replace `username` with your {% data variables.product.prodname_dotcom %} username. For example, if your username is `octocat`, the repository name should be `octocat.github.io`. ![Campo de nombre de repositorio](/assets/images/help/pages/create-repository-name-pages.png)
{% data reusables.repositories.sidebar-settings %}
{% data reusables.pages.sidebar-pages %}
1. Click **Choose a theme**. ![Elija un botón del tema](/assets/images/help/pages/choose-theme.png)
2. The Theme Chooser will open. Browse the available themes, then click **Select theme** to select a theme. It's easy to change your theme later, so if you're not sure, just choose one for now. ![Opciones de temas y botón Select theme (Seleccionar tema)](/assets/images/help/pages/select-theme.png)
3. After you select a theme, your repository's `README.md` file will open in the file editor. The `README.md` file is where you will write the content for your site. You can edit the file or keep the default content for now.
4. When you are done editing the file, click **Commit changes**.
5. Visit `username.github.io` to view your new website. **Nota:** Es posible que tome hasta 20 minutos la publicación de los cambios en tu sitio luego de que subes los cambios a {% data variables.product.product_name %}.

## Changing the title and description

By default, the title of your site is `username.github.io`. You can change the title by editing the `_config.yml` file in your repository. You can also add a description for your site.

1. Click the **Code** tab of your repository.
1. In the file list, click `_config.yml` to open the file.
1. Haz clic en {% octicon "pencil" aria-label="The edit icon" %} para editar el archivo.
1. The `_config.yml` file already contains a line that specifies the theme for your site. Add a new line with `title:` followed by the title you want. Add a new line with `description:` followed by the description you want. Por ejemplo:

   ```yaml
   theme: jekyll-theme-minimal
   title: Octocat's homepage
   description: Bookmark this to keep an eye on my project updates!
   ```

1. When you are done editing the file, click **Commit changes**.

## Siguientes pasos

Para obtener más información sobre cómo agregar páginas adicionales a tu sitio, consulta la sección "[Agregar contenido a tu sitio de GitHub Pages utilizando Jekyll](/pages/setting-up-a-github-pages-site-with-jekyll/adding-content-to-your-github-pages-site-using-jekyll#about-content-in-jekyll-sites)".

For more information about setting up a {% data variables.product.prodname_pages %} site with Jekyll, see "[About GitHub Pages and Jekyll](/pages/setting-up-a-github-pages-site-with-jekyll/about-github-pages-and-jekyll)."
