<script>
    import Modal from "./Modal.svelte";

    export let showModal = false;

	function handleClick() {
        showModal = !showModal;
        console.log(showModal)
    }
</script>

<div class="container">
    <div class="text-center">
        <h2>Stay in The Loop</h2>

        <p class="lead">Get the latest updates as they happen...</p>
    </div>

    <div class="row justify-content-center">
        <div class="col md-8 text-center">
            <p class="text-muted my-4">
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Nemo
                laboriosam ex at, architecto ab voluptatem saepe soluta amet
                nostrum aliquam eligendi explicabo vitae vel fugiat, fugit quis
                accusantium consequatur. Quas?
            </p>

            <button
                class="btn btn-primary"
                data-bs-toggle="modal"
                data-bs-target="#reg-modal"
                on:click={handleClick}
            >
                Register for Updates
            </button>
        </div>
    </div>
</div>

{#if showModal}
    <Modal on:click showModal />
{/if}