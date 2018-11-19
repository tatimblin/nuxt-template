<template>
    <div>
        <p>{{msg}}</p>
        <form name="contact" action="" method="post" netlify>
            <input type="hidden" name="form-name" value="contact" />
            <label class="form-label" for="name">
            Name:
            </label>
            <input class="form-field" name="name" id="name" />
            <label class="form-label" for="email">
            Email:
            </label>
            <input class="form-field" name="email" id="email" />
            <label class="form-label" for="message">
            Message:
            </label>
            <textarea class="form-field" name="message" id="message"></textarea>
            <input class="form-button" type="submit" value="Send message" />
        </form>
    </div>
</template>

<script>
export default {
    data() {
        return {
            msg: 'contact page',
            panelists: ['Evan You', 'Chris Fritz'],
            defaultPanelist: 'Evan You',
        };
    },
}
</script>
