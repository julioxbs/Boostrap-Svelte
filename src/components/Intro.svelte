<script>
    let smWidth = "";

    const tooltips = document.querySelectorAll(".tt");
    tooltips.forEach((t) => {
        new boostrap.Tooltip(t);
    });
</script>

<div class="container-lg" bind:clientWidth={smWidth}>
    <div class="row justify-content-center align-items-center">
        <div class="col-md-5 text-center text-md-start">
            <h1>
                <div class="display-2">Black-Belt</div>
                <div class="display-5 text-muted">Your Coding Skills</div>
            </h1>

            <p class="lead my-4 text-muted">
                Lorem ipsum dolor sit, amet consectetur adipisicing elit.
            </p>

            <a href="#pricing" class="btn btn-secondary btn-lg">Buy Now</a>

            <!-- Open sidebar / Offcanvas -->

            <a
                href="#sidebar"
                class="d-block mt-3"
                data-bs-toggle="offcanvas"
                role="button"
                aria-controls="sidebar"
            >
                Explore my other books
            </a>
        </div>

        {#if smWidth > 720}
            <div class="col-md-5 text-center">
                <!-- Tooltip -->
                <span
                    class="tt"
                    data-bs-placement="bottom"
                    title="Net Ninja Book COVER"
                >
                    <img
                        class="img-fluid"
                        src="/assets/ebook-cover.png"
                        alt="ebook"
                    />
                </span>
            </div>
        {/if}
    </div>
</div>

<!-- Offcanvas -->
<div
    class="offcanvas offcanvas-end"
    tabindex="-1"
    id="sidebar"
    aria-labelledby="sidebar-label"
>
    <div class="offcanvas-header">
        <h5 class="offcanvas-title text-center" id="sidebar-label">
            My Other Books
        </h5>
        <button
            class="btn-close"
            data-bs-dismiss="offcanvas"
            aria-label="Close"
        />
    </div>

    <div class="offcanvas-body">
        <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Nisi
            recusandae consectetur inventore accusamus dicta numquam magnam
            optio odio, obcaecati minima fuga modi eaque eligendi consequuntur
            deleniti, placeat facere. Quis, doloribus.
        </p>

        <!-- Dropdown -->
        <div class="dropdown mt-3">
            <button
                type="button"
                class="btn btn-secondary dropdown-toggle"
                id="book-dropdown"
                data-bs-toggle="dropdown">Choose a book title
            </button>

            <ul class="dropdown-menu" aria-labelledby="book-dropdown">
                <li><a href="..." class="dropdown-item">Become a React Superhero</a></li>
                <li><a href="..." class="dropdown-item">Conquering Vue.js</a></li>
                <li><a href="..." class="dropdown-item">Levelling up Your Next.js</a></li>
            </ul>
        </div>
    </div>
</div>
