<script>
  export let title, env;
</script>

<head>
  <meta charset='utf-8'>
  <meta name='viewport' content='width=device-width,initial-scale=1'>

  <title>{ title }</title>

  <base href="{env.baseurl}">
  <script type="module" src={env.entrypointJS + "/core/main.js?" + env.fingerprint}></script>

  <link href="https://fonts.googleapis.com/css2?family=Rubik:ital,wght@0,300;0,700;1,300&display=swap" rel="stylesheet">
  <link rel="icon" type="image/svg+xml" href="logo.svg">
  <link rel='stylesheet' href='global.css'>
  <link rel='stylesheet' href={env.entrypointJS + '/bundle.css?' + env.fingerprint}>
</head>
