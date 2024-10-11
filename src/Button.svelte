<script>
    export let variant = 'primary'; 
    export let label = 'Button';

</script>

<button
    class={`w-full max-w-xs m-8 p-5 h-12 rounded-md text-left flex items-center border border-red-500 
        ${variant === 'primary' ? 'bg-gray-100 text-black hover:bg-gray-200' : 
          variant === 'secondary' ? 'bg-gray-300 text-gray-800 hover:bg-gray-400' : 
          'bg-gray-200 text-red-800'}
        focus:outline none`} 

>
    {label}
    <div class="w-3 h-3 ml-2">
        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 9l-7 7-7-7"/>
        </svg>
    </div>
</button>
