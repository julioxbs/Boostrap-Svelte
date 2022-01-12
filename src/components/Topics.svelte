<script>
    let text =
        "The point of using Lorem Ipsum is that it has a more-or-less normal distribution of letters, as opposed to using 'Content here, content here', making it look like readable English. Many desktop publishing packages and web page editors now use Lorem Ipsum as their default model text";

    let items = [
        { title: "Chapter 1 - Your First Web Page", id: "one" },
        { title: "Chapter 2 - Mastering CSS", id: "two" },
        { title: "Chapter 3 - The Power of Javascript", id: "three" },
        { title: "Chapter 4 - Storing Data (Firebase Databases)", id: "four" },
        { title: "Chapter 5 - User Authentication", id: "five" },
    ];
</script>

<div class="container-md">
    <div class="text-center">
        <h2>Inside the Book...</h2>
        <p class="lead text-muted">A quick glance at the topics you'll learn</p>
    </div>

    <div class="row my-5 g-5 justify-content-around align-items-center">
        <div class="col-6 col-lg-4">
            <img src="/assets/kindle.png" alt="kindle" class="img-fluid" />
        </div>

        <div class="col-lg-6">
            <!-- Accordion -->
            <div class="accordion accordion-flush" id="chapters">
                {#each items as { title, id, index }}
                    <div class="accordion-item">
                        <h2 class="accordion-header" id="heading-{index + 1}">
                            <button
                                class="accordion-button collapsed"
                                type="button"
                                data-bs-toggle="collapse"
                                data-bs-target="#flush-collapse{id}"
                                aria-expanded="false"
                                aria-controls="flush-collapse{id}"
                            >
                                {title}
                            </button>
                        </h2>

                        <div
                            id="flush-collapse{id}"
                            class="accordion-collapse collapse"
                            aria-labelledby="heading-1"
                            data-bs-parent="#chapters"
                        >
                            <div class="accordion-body">
                                <p>{text}</p>
                                <p>{text}</p>
                            </div>
                        </div>
                    </div>
                {/each}
            </div>
        </div>
    </div>
</div>