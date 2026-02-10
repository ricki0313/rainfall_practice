# Reference
## -999.6 處理
- 氣象署與水量測器介紹: https://south.cwa.gov.tw/inner/meck1572422009QjcD
- -999.6 工程邏輯: https://w3fs.tainan.gov.tw/001/Upload/137/epaper/342/%E5%8F%B0%E7%81%A3%E5%9C%B0%E5%8D%80%E7%9F%AD%E5%BB%B6%E6%99%82%E5%BC%B7%E9%99%8D%E9%9B%A8%E4%BA%8B%E4%BB%B6%E6%B0%A3%E5%80%99%E7%89%B9%E6%80%A7%E5%88%86%E6%9E%90-%E8%BD%89%E8%BC%89%E5%9C%8B%E7%81%BD%E7%81%BD%E5%AE%B3%E9%98%B2%E6%95%91%E7%A7%91%E6%8A%80%E4%B8%AD%E5%BF%83%E7%81%BD%E5%AE%B3%E9%98%B2%E6%95%91%E9%9B%BB%E5%AD%90%E5%A0%B1%E7%AC%AC132.pdf
- -999.6 處理原則: WMO Guide to Climatological Practices (WMO-No.100) 2.4

## 繪製雨量圖參考方法: 
- 中央氣象署雨量網格化資料生產履歷: reference/雨量網格畫資料生產履歷.pdf
- station 資料: https://opendata.cwa.gov.tw/dataset/observation/O-A0002-001
- numpy 網格建立
    - linspace: https://ithelp.ithome.com.tw/articles/10233646
    - meshgrid: https://wangyeming.github.io/2018/11/12/numpy-meshgrid/

- Simple Kriging
    - Kriging Interpolation: https://hackmd.io/v77ZnZ6eQwOoqKMnfWkNgQ
    - reference/kriging.pdf

    - Fit Variogram: https://geostat-framework.readthedocs.io/projects/gstools/en/stable/examples/03_variogram/00_fit_variogram.html#sphx-glr-examples-03-variogram-00-fit-variogram-py

    - Spherical Model: https://geostat-framework.readthedocs.io/projects/gstools/en/stable/api/gstools.covmodel.Spherical.html#gstools.covmodel.Spherical
    - Simple Kriging: https://geostat-framework.readthedocs.io/projects/gstools/en/stable/examples/05_kriging/00_simple_kriging.html

- visualize
    - pcolormesh: https://matplotlib.net.cn/stable/gallery/images_contours_and_fields/pcolormesh_levels.html