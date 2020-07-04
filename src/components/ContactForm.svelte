<script>
    import { _, locale, locales } from 'svelte-i18n';
    
    import Deco from '../svg/3_deco.svelte';
    import Leaves from '../svg/3_leaves.svelte';
</script>

<form action="" class="form">
    <div class="form__group">
        <input type="text" class="form__control" placeholder={$_('form.name')}>
    </div>
    <div class="form__group">
        <input type="email" class="form__control" placeholder={$_('form.email')}>
    </div>
    <div class="form__group">
        <textarea class="form__control is-textarea" placeholder={$_('form.message')}></textarea>
    </div>
    <button type="submit" class="form__submit">{$_('form.cta')}</button>

    <Deco />
    <Leaves />
</form>

<style>
.form {
    position: relative;
    width: 100%;
}
.form__group + .form__group {
    margin-top: .5rem;
}
.form__control {
    border-radius: 2px;
    border: 2px solid #fff;
    background-color: #fff;
    box-shadow: none;
    color: #275E5E;
    font-family: Inter;
    font-weight: 400;
    font-size: .875rem;
    line-height: 1.5;
    padding: 1rem;
    width: 100%;
    transition: all .25s;
}
.form__control:focus,
.form__control:hover {
    border-color: #275E5E;
    outline:none;
}
.form__control.is-textarea {
    min-height: 15vh;
}
.form__submit {
    background-color: #4C8C40;
    border-radius: 2.5rem;
    padding: 1rem;
    border:none;
    font-family: Inter;
    font-weight: 600;
    color: #fff;
    margin-top: 1rem;
}

.form__submit:hover {
    background-color: #295d1f;
    outline:none;
    cursor:pointer;
}
</style>