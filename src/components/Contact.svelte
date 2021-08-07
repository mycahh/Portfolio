<section>
    <h3>Contact</h3>
    <form>
        <div class="form-group">
            <label for="name">Name</label>
            <input  placeholder="John Doe" id="name"/>
        </div>
        <div class="form-group">
            <label for="email">Email</label>
            <input type="email" placeholder="email@gmail.com" id="email"/>
        </div>
        <div class="form-group">
            <label for="message">Message</label>
            <textarea type="email" placeholder="Hello there!"/>
        </div>
        <button class="btn btn-primary">Submit</button>
    </form>
</section>

<style>
    section {
        padding: 2.5em 0;
        color: var(--gray900);
        width: 90%;
        margin: 0 auto;
    }

    h3 {
        text-align: center;
    }

    form {
        max-width: 464px;
        margin: 1.5rem auto;

        display: grid;
        gap: 2rem;
    }

    .form-group {
        display: flex;
        flex-direction: column;
    }

    label {
        margin-bottom: 6px;
        color: var(--form-label);
        font-weight: 500;
    }



    input {
        height: 3rem;
    }

    input, textarea {
        border: none;
        background: #ffffff;
        box-sizing: border-box;
        padding: 0.75rem;
        font-size: 16px;
        -webkit-box-shadow: 0px 0px 4px 1px rgba(0,0,0,0.12);
        box-shadow: 0px 0px 4px 1px rgba(0,0,0,0.12);
        font: inherit;
        border-radius: 6px;
    }

    input:focus {
        outline: none;
    }

    textarea {
        height: 140px;
    }

    input::placeholder, textarea::placeholder {
        color: #B8BCCA;
    }

    button {
        border: none;
        font: inherit;
        display: inline;
        margin-top: 1.2rem;
    }


</style>