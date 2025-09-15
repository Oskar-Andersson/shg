<div class="row scrollbar" style="flex: 1 1 auto; background-color: rgba(116,100,216, .0); overflow-y: auto;">                
    <div class="col-md-1"></div>
    <div class="col-md-10 d-flex flex-column" style="padding-top: 60px; ">        
        <div class="row" style="flex: 1 1 auto; " >
			<div class="col-md-12 d-flex flex-column" style="background-color: rgba(116,255,116, 0.0);">
                <slot></slot>            
			</div>
		</div>
    </div>
    <div class="col-md-1"></div>
</div>

<style>
/* Works on Firefox */
* {
  scrollbar-width: thin;
  scrollbar-color: rgb(223,184,152) rgb(29,36,43);
}

/* Works on Chrome, Edge, and Safari */
*::-webkit-scrollbar {
  width: 12px;
}

*::-webkit-scrollbar-track {
  background: rgb(29,36,43);
}

*::-webkit-scrollbar-thumb {
  background-color: rgb(223,184,152);
  border-radius: 20px;
  border: 3px solid rgb(29,36,43);
}
</style>