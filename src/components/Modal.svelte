<script>
    export let showModal = true;

    function closeBtn() {
        console.log(showModal);
    }
</script>

{#if showModal}
    <div class="modal fade" id="reg-modal">
        <div class="modal-dialog">
            <div class="modal-content">
                <div class="modal-header">
                    <h5 class="modal-title">Get the lastest updates</h5>

                    <button on:click={closeBtn} type="button" class="btn"
                        ><i class="bi bi-x-square-fill" /></button
                    >
                </div>

                <div class="modal-body">
                    <p>
                        Lorem ipsum dolor sit amet consectetur, adipisicing
                        elit. Quo aliquid iure nobis nulla! Dignissimos ea
                        assumenda, perspiciatis cumque autem ab cum quam
                        debitis, aut earum nostrum, vitae doloribus.
                        Consequuntur, voluptate?
                    </p>

                    <label for="modal-email" class="form-label">
                        Your email address:
                    </label>
                    <input
                        type="email"
                        class="form-control"
                        id="modal-email"
                        placeholder="e.g.mario@example.com"
                    />
                </div>

                <div class="modal-footer">
                    <button class="btn btn-primary"> Submit </button>
                </div>
            </div>
        </div>
    </div>
{/if}
