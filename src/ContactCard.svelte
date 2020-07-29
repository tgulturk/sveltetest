<style>

</style>

<script>
  export let userName;
  export let jobTitle;
  export let description;
  //export let imageUrl;

  const initialName = userName;
</script>

<div>
  <header>
    <!-- <div>
      <img src="{imageUrl}" alt="{userName}" />
    </div> -->
    <div>
      <h1>{userName} / {initialName}</h1>
      <h2>{jobTitle}</h2>
    </div>
  </header>
  <div>
    <p>{description}</p>
  </div>
</div>
