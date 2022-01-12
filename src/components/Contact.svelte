<div class="container-lg">
    <div class="text-center">
        <h2>Get in Touch</h2>

        <p class="lead">
            Questions to ask? Fill out the form to contact me directly...
        </p>
    </div>

    <div class="row justify-content-center my-5">
        <div class="col-lg-6">
            <form>
                <label for="email" class="form-label">Email address:</label>

                <div class="mb-4 input-group">
                    <span class="input-group-text">
                        <i class="bi bi-envelope"></i>
                    </span>

                    <input placeholder="e.g.mario@example.com" type="text" class="form-control" id="email">

                    <div class="input-group-text">
                        <span class="tt" data-bs-placement="bottom" title="Write your email">
                            <div class="bi bi-question-circle text-muted"></div>
                        </span>
                    </div>
                </div>

                <label for="name" class="form-label">Name:</label>

                <div class="mb-4 input-group">
                    <span class="input-group-text">
                        <i class="bi bi-chat-right-dots-fill"></i>
                    </span>

                    <input type="text" class="form-control" id="name" placeholder="e.g. Mario">

                    <div class="input-group-text">
                        <span class="tt" data-bs-placement="bottom" title="Pretty self explanatory realy...">
                            <div class="bi bi-question-circle text-muted"></div>
                        </span>
                    </div>
                </div>


                <label for="subject" class="form-label">
                    What is your question about?
                </label>

                <div class="input-group mb-4">
                    <span class="input-group-text">
                        <i class="bi bi-patch-question-fill"></i>
                    </span>

                    <select class="form-select">
                        <option value="pricing" selected>Pricing query</option>
                        <option value="content">Content query</option>
                        <option value="other">Other query</option>
                    </select>
                </div>

                <div class="form-floating mb-4 mt-2">
                    <textarea id="query" class="form-control" style="height: 140px;"></textarea>
                    <label for="query">Your query...</label>
                </div>

                <div class="mb-4 text-center">
                    <button type="submit" class="btn btn-secondary">
                        Submit
                    </button>
                </div>
            </form>
        </div>
    </div>
</div>