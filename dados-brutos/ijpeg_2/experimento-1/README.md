# comandos utilizados para o experimento 1

## cache separada

### `./sim-cache -cache:il1 il1:32:32:1:r -cache:dl1 dl1:32:32:1:r -cache:il2 none -cache:dl2 none -tlb:itlb none -tlb:dtlb none ./ijpeg.ss -image_file ./specmun.ppm -compression.quality 90 -compression.optimize_coding 0 -compression.smoothing_factor 90 -difference.image 1 -difference.x_stride 10 -difference.y_stride 10 -verbose 1 -GO.findoptcomp`

### a execução desse comando descreve duas caches separadas (uma para instruções e uma para dados) de um nível de hierarquia (somente L1)

## cache unificada

### `./sim-cache -cache:il1 dl1 -cache:dl1 ul1:64:32:1:r -cache:il2 none -cache:dl2 none -tlb:itlb none -tlb:dtlb none ./ijpeg.ss -image_file ./specmun.ppm -compression.quality 90 -compression.optimize_coding 0 -compression.smoothing_factor 90 -difference.image 1 -difference.x_stride 10 -difference.y_stride 10 -verbose 1 -GO.findoptcomp`

### a execução desse comando descreve uma cache unificada com o dobro de conjuntos para equivaler ao tamanho das duas caches separadas descritas no item anterior
