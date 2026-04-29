# comandos utilizados para o experimento 3

## usando uma cache unificada totalmente associativa de 64 blocos de 32 bytes cada

## método LRU

### `./sim-cache -cache:il1 dl1 -cache:dl1 ul1:1:32:64:l -cache:il2 none -cache:dl2 none -tlb:itlb none -tlb:dtlb none ./ijpeg.ss -image_file ./specmun.ppm -compression.quality 90 -compression.optimize_coding 0 -compression.smoothing_factor 90 -difference.image 1 -difference.x_stride 10 -difference.y_stride 10 -verbose 1 -GO.findoptcomp`

## método random

### `./sim-cache -cache:il1 dl1 -cache:dl1 ul1:1:32:64:r -cache:il2 none -cache:dl2 none -tlb:itlb none -tlb:dtlb none ./ijpeg.ss -image_file ./specmun.ppm -compression.quality 90 -compression.optimize_coding 0 -compression.smoothing_factor 90 -difference.image 1 -difference.x_stride 10 -difference.y_stride 10 -verbose 1 -GO.findoptcomp`

## método FIFO

### `./sim-cache -cache:il1 dl1 -cache:dl1 ul1:1:32:64:f -cache:il2 none -cache:dl2 none -tlb:itlb none -tlb:dtlb none ./ijpeg.ss -image_file ./specmun.ppm -compression.quality 90 -compression.optimize_coding 0 -compression.smoothing_factor 90 -difference.image 1 -difference.x_stride 10 -difference.y_stride 10 -verbose 1 -GO.findoptcomp`
