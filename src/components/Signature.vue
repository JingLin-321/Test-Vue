<template>
  <div>
    <div>
      <canvas id="signature-pad" class="signature-pad" width="400" height="200"></canvas>
    </div>
    <div>
      <button id="save">Save</button>
      <button id="clear">Clear</button>
    </div>
  </div>  
</template>

<script>
import SignaturePad from 'signature_pad'
export default {
  data() {
    return {
    };
  },
  mounted() {
    this.initPage();
  },
  methods: {
    initPage() {
      var signaturePad = new SignaturePad(document.getElementById('signature-pad'), {
        backgroundColor: 'rgba(255, 255, 255, 0)',
        penColor: 'rgb(0, 0, 0)'
      });
      var saveButton = document.getElementById('save');
      var cancelButton = document.getElementById('clear');

      saveButton.addEventListener('click', function (event) {
        var image = signaturePad.toDataURL('image/jpg');
      });

      cancelButton.addEventListener('click', function (event) {
        signaturePad.clear();
      });
    }
  }
};
</script>