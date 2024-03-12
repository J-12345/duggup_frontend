
<script>
  let buttonText = 'Follow';

  function changeText() {
    buttonText = buttonText === 'Follow' ? 'Followed' : 'Follow';
  }
</script>

<button on:click={changeText}
style="border:1px solid; border-bottom: 3px solid;"
class=" rounded-lg h-8 w-24 border-gray-700 hover:bg-blue-500 hover:text-white"
>
{buttonText}</button>
