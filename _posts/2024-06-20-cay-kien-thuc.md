---
title: Cây kiến thức
layout: single
classes: wide
mermaid: true
categories: duong-cua-dao
parent:
  label: Đường của đạo
  url: duong-cua-dao
---

![alt]({{ 'assets/images/dong-xi-yuan-pan-yuan-gu-shu-yuan-ying-tian.jpg' | absolute_url }})
> <cite>
<a target="_blank" href="https://dongxiyuan.artron.net/works_detail_brt000790000262">
董希源《盤垣古樹縁映天》- Đổng Tây Nguyên《Cổ thụ phản chiếu bầu trời》
</a>
</cite>

*Musk: One bit of advice: it is important to view knowledge as sort of a semantic tree — make sure you understand the fundamental principles, ie the trunk and big branches, before you get into the leaves/details or there is nothing for them to hang on to.*

> <cite><a target="_blank" href="https://fs.blog/elon-musk-knowledge/">
Elon Musk on How To Build Knowledge
</a></cite>

## Tính chất
Càng ở nhánh thì càng chi tiết. Càng lên cào thì càng trừu tượng, và tổng quát.\
Các nhánh con thì có những điểm chung và được tổng quát dần lên nhánh cha.

Cha con chỉ mang tính chất tương đối, và không chỉ có 1 cây duy nhất.\
Một nhánh con bên này có thể chung tính chất với 1 nhánh nào ở bên kia.\

Mục tiêu của người theo Đạo là càng lên cao càng tốt.\
Hoặc phủ càng nhiều càng tốt, tuy nhiên phủ nhiều ở lá mà không đi được lên cao thì cũng nguy hại đối với việc phát triển tư duy kiến thức.

Dưới đây là một số phương pháp có thể được dùng để bao phủ hay tiến tới mục tiêu.

## Tổng quát hóa (Bottom up)
Đây là phương pháp mà hay được áp dụng vào những năm đầu đi học khi người học chưa hề biết gì. Lúc này mọi kiến thức đều là mới. Quá trình này hầu hết mọi người đều rất quen thuộc và cũng rất ngán, vì nó là quá trình học cày ải. Đối với những người trẻ với việc học là ưu tiên số một thì đây là chuyện chấp nhận được.\
Tuy nhiên, với những người đã có công việc, việc phải học cái mới theo phương pháp này luôn là sự đánh đổi giữa trạng thái an toàn, và sự kỷ luật, cày ải của bản thân.

Một số lưu ý cần nhớ:
- Nhớ rằng cậu đang ở các nút lá, cố gắng tìm ra mục tiêu là nút cha phía trên, đừng để những chi tiết rối rắm làm mờ đi mục tiêu tổng quát hóa cuối cùng.
- <a target="_blank" href="https://martinfowler.com/bliki/ShuHaRi.html">Shu Ha Ri</a>: giúp cậu hiểu được quá trình theo từng giai đoạn một cách cụ thể.
- <a target="_blank" href="https://wei-he.xyz/5w">5W (Why --> How, What --> When, Where)</a>: giúp cậu định hình ra được những kiến thức nào cần phải chú ý, cần phải nhớ và có thể quên trong suốt quá trình học.

*Ví dụ sửa được các xe tay ga, cậu có thể học trước với sửa 1 dòng xe cụ thể như Lead, SH của Honda rồi sau đó tổng quát hóa nó lên thành Sửa xe tay ga.*

```mermaid
---
config:
  layout: elk
  look: handDrawn
---

flowchart LR
  subgraph 1[Cây kiến thức]
    direction TB
    tayga[Xe Tay Ga]
    lead[Honda Lead]
    sh[Honda SH]

    tayga-.-lead
    tayga-.-sh

    style tayga fill:#bbf,stroke:#f66,stroke-width:2px,color:#fff,stroke-dasharray: 5 5
  end

  subgraph 2[Quá trình]
    direction LR
    tayga2[Xe Tay Ga]
    lead2[Honda Lead]
    sh2[Honda SH]

    lead2-- Tổng quát (bottom up) ---tayga2
    sh2-- Tổng quát (bottom up) ---tayga2

    style tayga2 fill:#bbf,stroke:#f66,stroke-width:2px,color:#fff,stroke-dasharray: 5 5
  end
```

## Trên xuống (Top down)
Để học hay tìm hiểu 1 kiến thức mới, nếu may mắn bạn có thể áp dụng phương pháp top down. Thông thường đây là quá trình được diễn ra, hay thành quả đạt được sau khi bạn tổng quá hóa thành công. Đây là phương pháp rất phổ biến với những người đã học xong một chuyên môn nào đó và có đủ kinh nghiệm. Quá trình học một cái mới là quá trình gồm 2 bước chính:

- Dùng những kiến thức đã biết để tổng quát hóa lên nhánh cha (bottom up).
- Dùng kiến thức tổng quát đã được xây dựng và kiến thức chi tiết đã biết để liên hệ khi học một nhánh mới.

*Ví dụ để học sửa 1 loại xe mới như Yamaha Grande, sau khi đã biết sửa xe tay ga và Lead, SH.*

```mermaid
---
config:
  layout: elk
  look: handDrawn
---

flowchart LR
 subgraph 1[Cây kiến thức]
    direction TB
    tayga[Xe Tay Ga]
    lead[Honda Lead]
    sh[Honda SH]
    grande[Yamaha Grande]

    tayga-.-lead
    tayga-.-sh
    tayga-.-grande

    style grande fill:#bbf,stroke:#f66,stroke-width:2px,color:#fff,stroke-dasharray: 5 5
  end

  subgraph 2[Quá trình]
    direction LR
    tayga2[Xe Tay Ga]
    lead2[Honda Lead]
    sh2[Honda SH]
    grande2[Yamaha Grande]

    tayga2-- Trên xuống (topdown) ---grande2

    lead2-. Tham chiếu .-grande2
    sh2-.Tham chiếu .-grande2

    style grande2 fill:#bbf,stroke:#f66,stroke-width:2px,color:#fff,stroke-dasharray: 5 5
  end
```

## Tương phản (Jump)
Nếu với topdown và bottom up cậu sẽ mở rộng hay phát triển kiến thức ở gần mình. Mình sẽ là chuyên gia trong lĩnh vực của mình. Thì với tương phản, cậu sẽ chủ động mở rộng được kiến thức ở một nhánh cây hoàn toàn mới. Việc này sẽ giúp cậu không rơi vào trạng thái Tối ưu hóa cục bộ (local optimize). Mà sẽ giúp cho cậu có một cái nhìn nhiều chiều hơn một vấn đề nào đấy.

Tuy nhiên đây là một phương pháp nguy hiểm, vì nó không chỉ đòi hỏi nhiều thời gian công sức. Mà có thể dẫn người học tới trạng thái không có gì học ra hồn. Không chỉ vậy nó còn đòi hỏi cậu tại một số thời điểm quên đi những gì mình đã biết để có thể tiếp nhận được cái mới (mà có khi ngược lại hoàn toàn với cái cũ). Đây là một kỹ thuật khó vì nó trái ngược hoàn toàn với phản ứng tự nhiên của người học khi dùng những kiến thức đã biết để liên hệ lại (top down). <a target="_blank" href="https://www.oreilly.com/library/view/apprenticeship-patterns/9780596806842/ch02.html">Emptying the Cup</a> là kim chỉ nam với phương pháp này.

Thế nên tớ nghĩ phương pháp này chỉ phù hợp với những ai đã có một kiến thức nền nhất định và có ước muốn và động lực để tìm hiểu cái mới.

Tuy nhiên thành quả nhận lại sẽ rất tuyệt, cậu sẽ hiểu hơn về Đạo. Cậu sẽ tìm được sự cân bằng và một góc nhìn đa chiều hơn đối với 1 vấn đề cụ thể. Có thể thực hành được phương pháp này khả năng để thấy được đường của Đạo sẽ cao hơn ^^. 

```mermaid
---
config:
  look: handDrawn
---

flowchart
  d[Đạo] --- kt[Kỹ Thuật]
  kt[Kỹ Thuật] --- it[IT]
  kt[Kỹ Thuật] --- kt1[...]

  d[Đạo] --- kte[Kinh Tế]
  kte[Kinh Tế] --- macro[Vĩ Mô]
  kte[Kinh Tế] --- kte1[...]

  d[Đạo] --- d1[...]

  d[Đạo] --- xh[Xã hội]
  xh[Xã hội] --- xh1[...]
  xh[Xã hội] --- cs[Chính sách]

  style d fill:#bbf,stroke:#f66,stroke-width:2px,color:#fff,stroke-dasharray: 5 5
```

## Kết
Mỗi người đều có cho mình một hoặc nhiều cây kiến thức khác nhau. Mong cậu đừng trở thành một người bảo thủ, phiến diện hoặc ngược lại trở thành một người cái gì cũng biết mà thực ra là chả biết gì.

Hy vọng là cậu sẽ nhìn thấy, xây dựng được cây kiến thức của riêng mình. Tìm thấy được bản đồ trên con đường của Đạo.