<script>
  import Detail_1 from "../samIcon.png";
  import Detail_2 from "../detail-2.png";
  import Detail_3 from "../detail-3.png";
  import DetailedItem from "./detailedItem.svelte";
  import {
    simplifyYour,
    withXansam,
    theStrongest,
    xensonHas,
    oneSam,
    atXenson,
    enterpriseIn,
    theTrue
  } from "../constants";
</script>

<div class="sm:py-20">
  <DetailedItem
    Class="sm:grid sm:grid-cols-2 flex flex-col sm:px-20 px-5  items-center"
    IconImage={Detail_1}
    title={simplifyYour}
    detail={withXansam}
  />
  <DetailedItem
    Class="sm:grid sm:grid-cols-2 flex flex-col-reverse sm:px-20 px-5  items-center"
    IconImage={Detail_2}
    title={theStrongest}
    detail={xensonHas}
    reverse="true"
  />
  <DetailedItem
    Class="sm:grid sm:grid-cols-2 flex flex-col sm:px-20 px-5 items-center"
    IconImage={Detail_3}
    title={oneSam}
    detail={atXenson}
  />
  <DetailedItem
    Class="sm:grid sm:grid-cols-2 flex flex-col sm:px-20 px-5 items-center"
    title={enterpriseIn}
    detail={theTrue}
    reverse="true"
    
  />
</div>
