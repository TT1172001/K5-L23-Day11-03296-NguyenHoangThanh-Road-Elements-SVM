# Phiếu QC 1 — Road v1.0

Lô được kiểm (học viên): A01-A06        Người kiểm (học viên): Nguyễn Hoàng Thành 
Ngày: 20/11/2026                          Phiên bản guideline: Road v1.0  
File được kiểm (tên + `revision` trong manifest):  
Số ảnh kiểm: 6 (+ __ ảnh thêm, ghi riêng)   Số nhãn đã kiểm (shape + tag):  

## Tổng hợp theo mã
| Mã | Loại lỗi | Số mục kiểm | Số lỗi | Mức |
| --- | --- | ---: | ---: | --- |
| QC1-01 tag camera | sai thuộc tính / bỏ sót |  |  | nặng |
| QC1-02 đủ L1, R1 | bỏ sót |  |  | nặng |
| QC1-03 position | sai thuộc tính / thừa |  |  | nặng |
| QC1-04 tâm vạch, chiều, điểm dừng | sai phạm vi / bỏ sót |  |  | chính |
| QC1-05 vạch đứt, che | sai phạm vi / sai thuộc tính |  |  | chính |
| QC1-06 style, color, kind | sai thuộc tính |  |  | chính |
| QC1-07 vùng lái | sai phạm vi / bỏ sót / thừa |  |  | chính |
| QC1-08 đèn, màu | bỏ sót / sai phạm vi / sai thuộc tính |  |  | nặng / chính |
| QC1-09 facing, type, group, biển phụ | sai thuộc tính |  |  | chính |
| QC1-10 hình in, đủ biển | bỏ sót / sai phạm vi |  |  | chính |
| QC1-11 fisheye | sai phạm vi / sai thuộc tính |  |  | chính |
| QC1-12 file | lỗi file |  |  | nhẹ / nặng |

## Danh sách lỗi (mỗi lỗi một dòng)
| # | Mã | Ảnh | Nhãn (label, id) | Mức | Mô tả ngắn |
| --- | --- | --- | --- | --- | --- |
| 1 | QC1-03 | A01 | LANE34 | nặng | Position đúng là R1 nhưng lại đánh là L1 |
| 2 | QC1-03 | A02 | LANE38 | nặng | Position đúng là R1 nhưng lại đánh là L1 |
| 3 | QC1-03 | A02 | LANE38 | nặng | Style đúng là solid nhưng lại đánh là dashed |
| 4 | QC1-03 | A03 | LANE46 | nặng | Style đúng là solid nhưng lại đánh là dashed |
| 5 | QC1-10 | A03 | Traffic-sign 66 | chính | Group đúng là information nhưng lại đánh là prohibitory |
| 5 | QC1-10 | A03 | Traffic-sign 69 | chính | Group đúng là information nhưng lại đánh là prohibitory |
| 6 | QC1-10 | A03 | Traffic-sign 70 | chính | Group đúng là warning nhưng lại đánh là prohibitory |


## Ca mơ hồ
| Ảnh | Câu hỏi cho lead | Lời đáp (nếu có) |

## Quyết định
Lỗi nặng: 4   Lỗi chính: 3 / 72 nhãn = 4.17 %   Lỗi nhẹ: 0   Ca chờ lead: 0 
Quyết định (Release / Hold / Rework):  Rework
Lý do (theo luật của phiếu):  Có ít nhất 1 lỗi nặng

Loại lỗi: bỏ sót = thiếu nhãn phải có; thừa = gán cái không phải đối tượng; sai phạm vi = hình lệch, sai chiều, dừng sai chỗ, tràn vùng. Ba loại này theo cách chia lỗi gán nhãn của ISO/IEC 5259-4 (mục 8.4.2); "sai thuộc tính" và "lỗi file" là khóa học thêm. Cách xếp mức: [thang mức lỗi](../docs/qc_severity_road_v1.0.md).
