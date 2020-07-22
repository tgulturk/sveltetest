<style></style>

<script>
  export let userName;
  export let jobTitle;
  export let description;
  export let imageUrl;
</script>

<div>
  <header>
    <div>
        <img src="{imageUrl}" alt="{userName}" />
    </div>
    <div>
      <h1>{userName}</h1>
      <h2>{jobTitle}</h2>
    </div>
  </header>
  <div>
    <p>{description}</p>
  </div>
</div>
