# comandos utilizados para o experimento 2

## cache de tamanho 64 blocos

## mapeamento direto

### `./sim-cache -cache:il1 dl1 -cache:dl1 ul1:64:32:1:r -cache:il2 none -cache:dl2 none -tlb:itlb none -tlb:dtlb none ./ijpeg.ss -image_file ./specmun.ppm -compression.quality 90 -compression.optimize_coding 0 -compression.smoothing_factor 90 -difference.image 1 -difference.x_stride 10 -difference.y_stride 10 -verbose 1 -GO.findoptcomp`

### a execução desse comando descreve uma cache unificada de 64 blocos com mapeamento direto (64 conjuntos de uma via)

## totalmente associativo

### `./sim-cache -cache:il1 dl1 -cache:dl1 ul1:1:32:64:r -cache:il2 none -cache:dl2 none -tlb:itlb none -tlb:dtlb none ./ijpeg.ss -image_file ./specmun.ppm -compression.quality 90 -compression.optimize_coding 0 -compression.smoothing_factor 90 -difference.image 1 -difference.x_stride 10 -difference.y_stride 10 -verbose 1 -GO.findoptcomp`

### a execução desse comando descreve uma cache unificada de 64 blocos com mapeamento totalmente associativo (um conjunto com 64 vias)

## conjunto-associativa de duas vias (2-way)

### `./sim-cache -cache:il1 dl1 -cache:dl1 ul1:32:32:2:r -cache:il2 none -cache:dl2 none -tlb:itlb none -tlb:dtlb none ./ijpeg.ss -image_file ./specmun.ppm -compression.quality 90 -compression.optimize_coding 0 -compression.smoothing_factor 90 -difference.image 1 -difference.x_stride 10 -difference.y_stride 10 -verbose 1 -GO.findoptcomp`

### a execução desse comando descreve uma cache unificada de 64 blocos com mapeamento conjunto-associativo 2-way (32 conjuntos com 2 vias cada)

## conjunto-associativa de quatro vias (4-way)

### `./sim-cache -cache:il1 dl1 -cache:dl1 ul1:16:32:4:r -cache:il2 none -cache:dl2 none -tlb:itlb none -tlb:dtlb none ./ijpeg.ss -image_file ./specmun.ppm -compression.quality 90 -compression.optimize_coding 0 -compression.smoothing_factor 90 -difference.image 1 -difference.x_stride 10 -difference.y_stride 10 -verbose 1 -GO.findoptcomp`

### a execução desse comando descreve uma cache unificada de 64 blocos com mapeamento conjunto-associativo 4-way (16 conjuntos com 4 vias cada)

## conjunto-associativa de dezesseis vias (16-way)

### `./sim-cache -cache:il1 dl1 -cache:dl1 ul1:4:32:16:r -cache:il2 none -cache:dl2 none -tlb:itlb none -tlb:dtlb none ./ijpeg.ss -image_file ./specmun.ppm -compression.quality 90 -compression.optimize_coding 0 -compression.smoothing_factor 90 -difference.image 1 -difference.x_stride 10 -difference.y_stride 10 -verbose 1 -GO.findoptcomp`

### a execução desse comando descreve uma cache unificada de 64 blocos com mapeamento conjunto-associativo 16-way (4 conjuntos com 16 vias cada)