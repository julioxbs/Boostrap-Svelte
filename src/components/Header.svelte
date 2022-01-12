<script>
    let navBar;

    let linksNames = [
        {title: "About The Book", href: "#intro"},
        {title: "Reviews", href: "#"},
        {title: "Get in Touch", href: "#topics"},
        {title: "Pricing", href: "#pricing"},
    ]

    function toggle() {
        navBar.classList.toggle("d-block")
    }
</script>

<nav class="navbar navbar-expand-md navbar-light">
    <div class="container-xl">
        <a href="#intro" class="navbar-brand">
            <span class="fw-bold text-secondary">
                <i class="bi bi-book-half"></i>
                Net Ninja Pro - The book
            </span>
        </a>

        <!-- Toggle Button for mobile nav -->
        <button on:click={toggle} class="navbar-toggler" type="button">
            <span class="navbar-toggler-icon" />
        </button>

        <!-- Navbar Links -->
        <div
            bind:this={navBar}
            class="collapse navbar-collapse justify-content-end align-center"
            id="main-nav"
        >
            <ul class="navbar-nav">
                {#each linksNames as {title, href}}
                    <li class="nav-item">
                        <a class="nav-link" href="{href}">{title.toUpperCase()}</a>
                    </li>
                {/each}

                <li class="nav-item ms-2 d-none d-md-inline">
                    <a href="#" class="btn btn-secondary">BUY NOW </a>
                </li>
            </ul>
        </div>
    </div>
</nav>
