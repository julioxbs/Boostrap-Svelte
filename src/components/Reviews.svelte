<script>
    let text =
        "Lorem ipsum dolor sit amet consectetur adipisicing elit. Incidunt facilis, beatae animi explicabo modi voluptatum porro quidem laborum accusamus eveniet sed quaerat vel tempore. Quasi quaerat laborum minus eum doloribus.";

    let listsItems = [
        {
            title: "A must buy for every aspiring web dev",
            by: "Review by Mario",
        },
        {
            title: "A must buy for every aspiring web dev",
            by: "Review by Mario",
        },
        {
            title: "A must buy for every aspiring web dev",
            by: "Review by Mario",
        },
    ];
</script>

<div class="container-lg">
    <div class="text-center">
        <h2><i class="bi bi-stars"></i> Book Reviews</h2>

        <p class="lead">What my students have said about book...</p>
    </div>

    <div class="row justify-content-center my-5">
        <div class="col-lg-8">
            <div class="list-group">
                {#each listsItems as { title, by }}
                    <div class="list-group-item py-3">
                        <h5 class="mb-1 text-center">{title}</h5>

                        <p class="mb-1">{text}</p>

                        <small>{by}</small>
                    </div>
                {/each}
            </div>
        </div>
    </div>
</div>

<style>
    .bi-stars {
        color: yellow;
    }
</style>