<div class="col">
    <div class="card h-100 bg bg-transparent">
        <slot name='img'>
            <img src="https://user-images.githubusercontent.com/43302778/106805462-7a908400-6645-11eb-958f-cd72b74a17b3.jpg" class="card-img-top" alt=''>
        </slot>
        <div class="card-body">
            <slot name='title'>
                <h5 class="card-title">Nothing</h5>
            </slot>
            <slot name='text'>
                <p class="card-text">Something...</p>
            </slot>
        </div>
    </div>
</div>