<script>
  import { beforeNavigate } from '$app/navigation';
  beforeNavigate(() => {
  const button = document.querySelector('button.navbar-toggler:not(.collapsed)[aria-expanded="true"]');
  if (button) {
    button.click(); // Trigger the click event
  }
});


</script>

<nav class="navbar navbar-expand-lg bg-body-tertiary">
  <div class="container-fluid">
    <a class="navbar-brand" href="/">Navbar</a>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNavDropdown" aria-controls="navbarNavDropdown" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarNavDropdown">
      <ul class="navbar-nav">
        <li class="nav-item">
          <a class="nav-link active" aria-current="page" href="/">Home</a>
        </li>

        <!-- Link to /dropdown route -->
        <li class="nav-item">
          <a class="nav-link" href="/dropdown">Dropdown</a>
        </li>

        <!-- Link to /modal route -->
        <li class="nav-item">
          <a class="nav-link" href="/modal">Modal</a>
        </li>

        <li class="nav-item dropdown">
          <a class="nav-link dropdown-toggle" href="#" role="button" data-bs-toggle="dropdown" aria-expanded="false">
            Test
          </a>
          <ul class="dropdown-menu">
            <li><a class="dropdown-item" href="#">Test Action 1</a></li>
            <li><a class="dropdown-item" href="#">Test Action 2</a></li>
            <li><a class="dropdown-item" href="#">Another Test</a></li>
          </ul>
        </li>
      </ul>
    </div>
  </div>
</nav>

  