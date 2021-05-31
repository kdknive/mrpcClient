<template>
    <div class="simulasi-container grid col-auto p-0 m-0">
        <div class="simulasi-container-horizontal grid text-white text-left font-bold m-1 p-0 align-middle text-xs lg:text-xl">
            <p>Komponen</p>
            <p>Nama Komponen</p>
            <p>Harga</p>
        </div>
        <div class="simulasi-container-horizontal text-xs lg:text-xl">
            <p>CPU</p>
            <div class="komp-selection">
                <label for="cpu"></label>
                    <select v-model="cpuSelect" name="cpu" id="cpu" class="form-control" tabindex="12">
                        <option value="" selected disabled hidden>Choose CPU</option>
                        <option v-for="cpu in cpus" :key="cpu.id">{{ cpu.Name }}</option>
                    </select>
            </div>
            <p>Rp.x.xxx.xxx</p>
        </div>
        <div class="simulasi-container-horizontal text-xs lg:text-xl">
            <p>Motherboard</p>
            <div class="komp-selection">
                <label for="motherboard"></label>
                    <select v-model="cpuSelect" id="motherboard" name="motherboard" class="form-control" tabindex="12">
                        <option value="" selected disabled hidden>Choose Motherboard</option>
                        <option v-for="cpu in cpus" :key="cpu.id">{{ cpu.Name }}</option>
                    </select>
            </div>
            <p>Rp.x.xxx.xxx</p>
        </div>
        <div class="simulasi-container-horizontal text-xs lg:text-xl">
            <p>Memory</p>
            <div class="komp-selection">
                <label for="memory"></label>
                    <select v-model="cpuSelect" id="memory" name="memory" class="form-control" tabindex="12">
                        <option value="" selected disabled hidden>Choose Memory</option>
                        <option v-for="cpu in cpus" :key="cpu.id">{{ cpu.Name }}</option>
                    </select>
            </div>
            <p>Rp.x.xxx.xxx</p>
        </div>  
        <div class="simulasi-container-horizontal text-xs lg:text-xl">
            <p>Graphics Card</p>
            <div class="komp-selection">
                <label for="graphicsCard"></label>
                    <select v-model="cpuSelect" id="graphicsCard" name="graphicsCard" class="form-control" tabindex="12">
                        <option value="" selected disabled hidden>Choose Graphics Card</option>
                        <option v-for="cpu in cpus" :key="cpu.id">{{ cpu.Name }}</option>
                    </select>
            </div>
            <p>Rp.x.xxx.xxx</p>
        </div>
        <div class="simulasi-container-horizontal text-xs lg:text-xl">
            <p>Power Supply</p>
            <div class="komp-selection">
                <label for="powerSupply"></label>
                    <select v-model="cpuSelect" id="powerSupply" name="powerSupply" class="form-control" tabindex="12">
                        <option value="" selected disabled hidden>Choose Power Supply</option>
                        <option v-for="cpu in cpus" :key="cpu.id">{{ cpu.Name }}</option>
                    </select>
            </div>
            <p>Rp.x.xxx.xxx</p>
        </div>
        <div class="simulasi-container-horizontal text-xs lg:text-xl">
            <p>Case</p>
            <div class="komp-selection">
                <label for="case"></label>
                    <select v-model="cpuSelect" id="case" name="case" class="form-control" tabindex="12">
                        <option value="" selected disabled hidden>Choose Case</option>
                        <option v-for="cpu in cpus" :key="cpu.id">{{ cpu.Name }}</option>
                    </select>
            </div>
            <p>Rp.x.xxx.xxx</p>
        </div> 
        <div class="simulasi-container-horizontal text-xs lg:text-xl">
            <p>Hard Drive 1</p>
            <div class="komp-selection">
                <label for="hardDrive"></label>
                    <select v-model="cpuSelect" id="hardDrive" name="hardDrive" class="form-control" tabindex="12">
                        <option value="" selected disabled hidden>Choose Hard Drive</option>
                        <option v-for="cpu in cpus" :key="cpu.id">{{ cpu.Name }}</option>
                    </select>
            </div>
            <p>Rp.x.xxx.xxx</p>
        </div> 
        <div class="simulasi-container-horizontal text-xs lg:text-xl">
            <p>Hard Drive 2</p>
            <div class="komp-selection">
                <label for="hardDrive"></label>
                    <select v-model="cpuSelect" id="hardDrive" name="hardDrive" class="form-control" tabindex="12">
                        <option value="" selected disabled hidden>Choose Hard Drive</option>
                        <option v-for="cpu in cpus" :key="cpu.id">{{ cpu.Name }}</option>
                    </select>
            </div>
            <p>Rp.x.xxx.xxx</p>
        </div> 
        <div class="simulasi-container-horizontal text-xs lg:text-xl">
            <p>Hard Drive 3</p>
            <div class="komp-selection">
                <label for="hardDrive"></label>
                    <select v-model="cpuSelect" id="hardDrive" name="hardDrive" class="form-control" tabindex="12">
                        <option value="" selected disabled hidden>Choose Hard Drive</option>
                        <option v-for="cpu in cpus" :key="cpu.id">{{ cpu.Name }}</option>
                    </select>
            </div>
            <p>Rp.x.xxx.xxx</p>
        </div> 
        <div class="simulasi-container-horizontal text-xs lg:text-xl">
            <p>Keyboard</p>
            <div class="komp-selection">
                <label for="keyboard"></label>
                    <select v-model="cpuSelect" id="keyboard" name="keyboard" class="form-control" tabindex="12">
                        <option value="" selected disabled hidden>Choose Keyboard</option>
                        <option v-for="cpu in cpus" :key="cpu.id">{{ cpu.Name }}</option>
                    </select>
            </div>
            <p>Rp.x.xxx.xxx</p>
        </div>
        <div class="simulasi-container-horizontal text-xs lg:text-xl">
            <p>Mouse</p>
            <div class="komp-selection">
                <label for="mouse"></label>
                    <select v-model="cpuSelect" id="mouse" name="mouse" class="form-control" tabindex="12">
                        <option value="" selected disabled hidden>Choose Mouse</option>
                        <option v-for="cpu in cpus" :key="cpu.id">{{ cpu.Name }}</option>
                    </select>
            </div>
            <p>Rp.x.xxx.xxx</p>
        </div>
        <div class="simulasi-container-horizontal text-xs lg:text-xl">
            <p>Monitor</p>
            <div class="komp-selection">
                <label for="monitor"></label>
                    <select v-model="cpuSelect" id="monitor" name="monitor" class="form-control" tabindex="12">
                        <option value="" selected disabled hidden>Choose Monitor</option>
                        <option v-for="cpu in cpus" :key="cpu.id">{{ cpu.Name }}</option>
                    </select>
            </div>
            <p>Rp.x.xxx.xxx</p>
        </div>
        <div class="simulasi-container-horizontal text-xs lg:text-xl">
            <p>CPU Cooler</p>
            <div class="komp-selection">
                <label for="cpuCooler"></label>
                    <select v-model="cpuSelect" id="cpuCooler" name="cpuCooler" class="form-control" tabindex="12">
                        <option value="" selected disabled hidden>Choose CPU Cooler</option>
                        <option v-for="cpu in cpus" :key="cpu.id">{{ cpu.Name }}</option>
                    </select>
            </div>
            <p>Rp.x.xxx.xxx</p>
        </div>
        <div class="simulasi-container-horizontal text-xs lg:text-xl">
            <p>Case Fan</p>
            <div class="komp-selection">
                <label for="caseFan"></label>
                    <select v-model="cpuSelect" id="caseFan" name="caseFan" class="form-control" tabindex="12">
                        <option value="" selected disabled hidden>Choose Case Fan</option>
                        <option v-for="cpu in cpus" :key="cpu.id">{{ cpu.Name }}</option>
                    </select>
            </div>
            <p>Rp.x.xxx.xxx</p>
        </div>
        <div class="simulasi-container-horizontal text-xs lg:text-xl">
            <p>Wireless Network Card</p>
            <div class="komp-selection">
                <label for="wirelessNetworkCard"></label>
                    <select v-model="cpuSelect" id="wirelessNetworkCard" name="wirelessNetworkCard" class="form-control" tabindex="12">
                        <option value="" selected disabled hidden>Choose Wireless Network Card</option>
                        <option v-for="cpu in cpus" :key="cpu.id">{{ cpu.Name }}</option>
                    </select>
            </div>
            <p>Rp.x.xxx.xxx</p>
        </div>
        <div class="simulasi-container-horizontal text-xs lg:text-xl">
            <p>Wired Network Card</p>
            <div class="komp-selection">
                <label for="wiredNetworkCard"></label>
                    <select v-model="cpuSelect" id="wiredNetworkCard" name="wiredNetworkCard" class="form-control" tabindex="12">
                        <option value="" selected disabled hidden>Choose Wired Network Card</option>
                        <option v-for="cpu in cpus" :key="cpu.id">{{ cpu.Name }}</option>
                    </select>
            </div>
            <p>Rp.x.xxx.xxx</p>
        </div>
        <div class="simulasi-container-horizontal text-xs lg:text-xl">
            <p>Optical Drive</p>
            <div class="komp-selection">
                <label for="opticalDrive"></label>
                    <select v-model="cpuSelect" id="opticalDrive" name="opticalDrive" class="form-control" tabindex="12">
                        <option value="" selected disabled hidden>Choose Optical Drive</option>
                        <option v-for="cpu in cpus" :key="cpu.id">{{ cpu.Name }}</option>
                    </select>
            </div>
            <p>Rp.x.xxx.xxx</p>
        </div>
        <div class="simulasi-container-horizontal text-xs lg:text-xl">
            <p>Sound Card</p>
            <div class="komp-selection">
                <label for="soundCard"></label>
                    <select v-model="cpuSelect" id="soundCard" name="soundCard" class="form-control" tabindex="12">
                        <option value="" selected disabled hidden>Choose Sound Card</option>
                        <option v-for="cpu in cpus" :key="cpu.id">{{ cpu.Name }}</option>
                    </select>
            </div>
            <p>Rp.x.xxx.xxx</p>
        </div>
        <div class="simulasi-container-horizontal text-xs lg:text-xl">
            <p>Speakers</p>
            <div class="komp-selection">
                <label for="speakers"></label>
                    <select v-model="cpuSelect" id="speakers" name="speakers" class="form-control" tabindex="12">
                        <option value="" selected disabled hidden>Choose Speakers</option>
                        <option v-for="cpu in cpus" :key="cpu.id">{{ cpu.Name }}</option>
                    </select>
            </div>
            <p>Rp.x.xxx.xxx</p>
        </div>
        <div class="simulasi-container-horizontal text-xs lg:text-xl">
            <p>Headphones</p>
            <div class="komp-selection">
                <label for="headphones"></label>
                    <select v-model="cpuSelect" id="headphones" name="headphones" class="form-control" tabindex="12">
                        <option value="" selected disabled hidden>Choose Headphones</option>
                        <option v-for="cpu in cpus" :key="cpu.id">{{ cpu.Name }}</option>
                    </select>
            </div>
            <p>Rp.x.xxx.xxx</p>
        </div>
        <div class="simulasi-container-horizontal text-xs lg:text-xl">
            <p>UPS</p>
            <div class="komp-selection">
                <label for="ups"></label>
                    <select v-model="cpuSelect" id="ups" name="ups" class="form-control" tabindex="12">
                        <option value="" selected disabled hidden>Choose UPS</option>
                        <option v-for="cpu in cpus" :key="cpu.id">{{ cpu.Name }}</option>
                    </select>
            </div>
            <p>Rp.x.xxx.xxx</p>
        </div>
        <div class="simulasi-container-horizontal text-xs lg:text-xl">
            <p>Thermal Paste</p>
            <div class="komp-selection">
                <label for="thermalPaste"></label>
                    <select v-model="cpuSelect" id="thermalPaste" name="thermalPaste" class="form-control" tabindex="12">
                        <option value="" selected disabled hidden>Choose Thermal Paste</option>
                        <option v-for="cpu in cpus" :key="cpu.id">{{ cpu.Name }}</option>
                    </select>
            </div>
            <p>Rp.x.xxx.xxx</p>
        </div>
    </div>
        <button  @click="() => ToggleSave('buttonTrigger')" class="saveBuild-btn text-black w-full h-12 bg-green1 my-5 text-center inline-block text-xl cursor-pointer ">Save Build</button> 
        <SavePop v-if="saveTriggers.buttonTrigger" :ToggleSave="() => ToggleSave('buttonTrigger')" ></SavePop>
</template>

<script>
import { ref } from 'vue'

export default{
    
}
</script>

<script setup>
import SavePop from './SavePop.vue'

const saveTriggers = ref({
    buttonTrigger:false
});

const ToggleSave = (trigger) => {
    saveTriggers.value[trigger] = !saveTriggers.value[trigger]
}
</script>

<style scoped>

.simulasi-container-horizontal{
    grid-template-columns: 20% 60% 20%;
    font-family: 'Roboto', sans-serif;
    font-weight: 400;
}

.simluasi-boldtext{
    font-weight: 700;
}

.komp-selection option, .komp-selection select{
    background-color: black;
    color: white;
    border: none;
    width: 95%;
    height: 100%;
    font-family: 'Roboto', sans-serif;
    font-weight: 400;
    /* font-size: 18px; */
}

.simulasi-container-horizontal{
    display: grid;
    grid-template-columns: 20% 60% 20%;
    color: white;
    font-family: 'Roboto', sans-serif;
    font-weight: 400;
    /* font-size: 18px; */
    text-align: left;
    margin: 1rem 0;
    padding: 3px 0;
    vertical-align: middle;
    align-items: center;
}
</style>