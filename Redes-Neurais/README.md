# Projeto Final - Modelos Preditivos Conexionistas

### Rute Alves da Cunha

|**Tipo de Projeto**|**Modelo Selecionado**|**Linguagem**|
|--|--|--|
| Detecção de Objetos | YOLOv5m | PyTorch |

O objetivo do projeto foi identificar se uma pessoa está usando capacete de construção civil corretamente ou não. Para tal, foram capturadas, da internet, no mínimo 75 imagens de cada classe conforme disposição a seguir:

   - Pessoas usando capacete de construção civil (helmet)
   - Pessoas usando outros acessórios na cabeça (hats)
   - Pessoas sem nada na cabeça (nothing)
   - Pessoas calvas (bald)

## Performance

O modelo treinado possui performance de **90,97%**.

### Output do bloco de treinamento

<details>
  <summary>Click to expand!</summary>
  
  ```text
    Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
      0/999      10.4G     0.1151    0.03037    0.04685         60        640: 100% 10/10 [00:10<00:00,  1.09s/it]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:03<00:00,  1.75s/it]
                   all        100        196    0.00101      0.242    0.00114    0.00033

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
      1/999      12.4G    0.08908    0.03366    0.04269         78        640: 100% 10/10 [00:05<00:00,  1.73it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.29it/s]
                   all        100        196    0.00455       0.71     0.0112    0.00313

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
      2/999      12.4G    0.07294    0.03505    0.03666         91        640: 100% 10/10 [00:06<00:00,  1.64it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.37it/s]
                   all        100        196      0.598      0.169     0.0897     0.0267

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
      3/999      12.4G    0.06641    0.02973    0.03355         90        640: 100% 10/10 [00:05<00:00,  1.78it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.23it/s]
                   all        100        196      0.122      0.371      0.124     0.0479

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
      4/999      12.4G    0.06595    0.02661    0.03192         73        640: 100% 10/10 [00:05<00:00,  1.72it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.51it/s]
                   all        100        196      0.085      0.269      0.142     0.0462

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
      5/999      12.4G    0.06685    0.02527    0.02942         65        640: 100% 10/10 [00:05<00:00,  1.73it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.25it/s]
                   all        100        196        0.3      0.447      0.277     0.0966

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
      6/999      12.4G    0.06703    0.02361    0.02681         76        640: 100% 10/10 [00:05<00:00,  1.77it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.54it/s]
                   all        100        196      0.179      0.396      0.218     0.0972

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
      7/999      12.4G     0.0689    0.02281     0.0222         55        640: 100% 10/10 [00:05<00:00,  1.68it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.25it/s]
                   all        100        196      0.286      0.519      0.298      0.129

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
      8/999      12.4G    0.06561    0.02093    0.01806         75        640: 100% 10/10 [00:05<00:00,  1.79it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.58it/s]
                   all        100        196      0.305      0.494      0.312      0.126

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
      9/999      12.4G    0.06365    0.01916    0.01632         80        640: 100% 10/10 [00:06<00:00,  1.67it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.32it/s]
                   all        100        196      0.361      0.512      0.376      0.159

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     10/999      12.4G    0.06107      0.019    0.01539         77        640: 100% 10/10 [00:05<00:00,  1.78it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.58it/s]
                   all        100        196      0.453      0.506      0.458      0.176

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     11/999      12.4G    0.05788    0.01678    0.01353         75        640: 100% 10/10 [00:06<00:00,  1.62it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.49it/s]
                   all        100        196      0.424      0.531      0.443       0.21

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     12/999      12.4G     0.0558     0.0175    0.01201         77        640: 100% 10/10 [00:05<00:00,  1.77it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.57it/s]
                   all        100        196      0.417      0.527      0.495      0.198

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     13/999      12.4G     0.0543    0.01637    0.01051         75        640: 100% 10/10 [00:06<00:00,  1.60it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.57it/s]
                   all        100        196      0.435      0.529      0.513       0.25

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     14/999      12.4G    0.05073    0.01541   0.008912         79        640: 100% 10/10 [00:05<00:00,  1.76it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.57it/s]
                   all        100        196      0.566      0.671      0.642      0.307

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     15/999      12.4G    0.04755    0.01557   0.008865         73        640: 100% 10/10 [00:06<00:00,  1.60it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.55it/s]
                   all        100        196      0.558      0.676       0.63      0.322

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     16/999      12.4G    0.04722    0.01437     0.0089         82        640: 100% 10/10 [00:05<00:00,  1.74it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.31it/s]
                   all        100        196      0.335      0.755      0.538      0.249

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     17/999      12.4G    0.04711    0.01537   0.007612         70        640: 100% 10/10 [00:06<00:00,  1.64it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.55it/s]
                   all        100        196      0.552      0.647      0.621      0.259

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     18/999      12.4G    0.04504    0.01498   0.007438         68        640: 100% 10/10 [00:05<00:00,  1.72it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.31it/s]
                   all        100        196      0.626      0.645       0.67       0.31

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     19/999      12.4G    0.04395      0.015   0.008301         71        640: 100% 10/10 [00:06<00:00,  1.65it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.53it/s]
                   all        100        196      0.696      0.722      0.734      0.333

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     20/999      12.4G     0.0443    0.01467   0.006486        104        640: 100% 10/10 [00:06<00:00,  1.66it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.27it/s]
                   all        100        196      0.661      0.748      0.705      0.336

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     21/999      12.4G    0.04399    0.01586   0.006873         77        640: 100% 10/10 [00:06<00:00,  1.66it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.52it/s]
                   all        100        196      0.595      0.746       0.68      0.311

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     22/999      12.4G    0.04253    0.01409   0.006454         78        640: 100% 10/10 [00:06<00:00,  1.63it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.32it/s]
                   all        100        196      0.677       0.66      0.696      0.328

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     23/999      12.4G    0.04204    0.01477   0.006056         55        640: 100% 10/10 [00:05<00:00,  1.70it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.53it/s]
                   all        100        196      0.792      0.686      0.744      0.348

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     24/999      12.4G    0.04183    0.01448   0.005089         65        640: 100% 10/10 [00:06<00:00,  1.60it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.39it/s]
                   all        100        196      0.502      0.575      0.502      0.208

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     25/999      12.4G    0.04056    0.01517   0.007547         65        640: 100% 10/10 [00:05<00:00,  1.71it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.56it/s]
                   all        100        196      0.596      0.679      0.603      0.298

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     26/999      12.4G    0.04047    0.01327   0.007719         48        640: 100% 10/10 [00:06<00:00,  1.59it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.37it/s]
                   all        100        196      0.627       0.65      0.666      0.328

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     27/999      12.4G    0.04057    0.01461   0.006578         62        640: 100% 10/10 [00:05<00:00,  1.71it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.55it/s]
                   all        100        196      0.729      0.783      0.802      0.413

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     28/999      12.4G    0.04021    0.01238   0.005579         64        640: 100% 10/10 [00:06<00:00,  1.61it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.52it/s]
                   all        100        196      0.747      0.736      0.765      0.379

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     29/999      12.4G    0.03925    0.01374   0.004729         68        640: 100% 10/10 [00:05<00:00,  1.71it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.51it/s]
                   all        100        196      0.712      0.671       0.73      0.344

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     30/999      12.4G    0.03936    0.01396   0.005576         64        640: 100% 10/10 [00:06<00:00,  1.58it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.56it/s]
                   all        100        196      0.801      0.684      0.776      0.398

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     31/999      12.4G    0.03638    0.01371    0.00533         59        640: 100% 10/10 [00:05<00:00,  1.70it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.54it/s]
                   all        100        196      0.765      0.709      0.751      0.357

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     32/999      12.4G    0.03817     0.0141   0.004986         85        640: 100% 10/10 [00:06<00:00,  1.57it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.54it/s]
                   all        100        196      0.748      0.764      0.795      0.418

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     33/999      12.4G    0.03751    0.01182   0.005546         69        640: 100% 10/10 [00:05<00:00,  1.70it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.52it/s]
                   all        100        196      0.819       0.69      0.787       0.34

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     34/999      12.4G    0.03709    0.01376    0.00448         60        640: 100% 10/10 [00:06<00:00,  1.59it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.51it/s]
                   all        100        196      0.723      0.792      0.784       0.41

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     35/999      12.4G    0.03653    0.01352   0.004618         69        640: 100% 10/10 [00:05<00:00,  1.70it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.54it/s]
                   all        100        196      0.696      0.767      0.789      0.391

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     36/999      12.4G      0.036    0.01272   0.005561         69        640: 100% 10/10 [00:06<00:00,  1.58it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.58it/s]
                   all        100        196      0.837      0.839       0.87      0.436

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     37/999      12.4G    0.03733    0.01485   0.004954         70        640: 100% 10/10 [00:05<00:00,  1.70it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.44it/s]
                   all        100        196       0.84       0.79      0.836      0.422

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     38/999      12.4G    0.03644    0.01364   0.005221         91        640: 100% 10/10 [00:06<00:00,  1.61it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.54it/s]
                   all        100        196      0.809      0.738        0.8      0.419

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     39/999      12.4G    0.03606    0.01385   0.005618         60        640: 100% 10/10 [00:05<00:00,  1.71it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.48it/s]
                   all        100        196      0.802      0.727      0.762      0.369

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     40/999      12.4G    0.03667    0.01394   0.004768         88        640: 100% 10/10 [00:06<00:00,  1.62it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.56it/s]
                   all        100        196      0.806      0.757        0.8      0.403

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     41/999      12.4G    0.03501    0.01322    0.00474         60        640: 100% 10/10 [00:05<00:00,  1.70it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.38it/s]
                   all        100        196      0.718      0.776      0.715      0.349

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     42/999      12.4G    0.03557    0.01291   0.003962         62        640: 100% 10/10 [00:06<00:00,  1.61it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.56it/s]
                   all        100        196      0.877      0.835      0.883      0.435

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     43/999      12.4G    0.03445    0.01299   0.004116         62        640: 100% 10/10 [00:05<00:00,  1.67it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.33it/s]
                   all        100        196      0.883      0.806       0.89      0.451

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     44/999      12.4G      0.035    0.01273   0.003915         83        640: 100% 10/10 [00:06<00:00,  1.66it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.55it/s]
                   all        100        196      0.882      0.789      0.891      0.465

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     45/999      12.4G    0.03403    0.01258    0.00468         64        640: 100% 10/10 [00:06<00:00,  1.62it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.31it/s]
                   all        100        196      0.894      0.797      0.879      0.456

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     46/999      12.4G    0.03285     0.0125   0.003847         67        640: 100% 10/10 [00:05<00:00,  1.70it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.56it/s]
                   all        100        196      0.823      0.763      0.811      0.385

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     47/999      12.4G    0.03534    0.01323   0.004551         64        640: 100% 10/10 [00:06<00:00,  1.62it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.33it/s]
                   all        100        196      0.824      0.733      0.822      0.407

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     48/999      12.4G    0.03424    0.01272   0.003925         87        640: 100% 10/10 [00:05<00:00,  1.70it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.55it/s]
                   all        100        196      0.804       0.82      0.869      0.448

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     49/999      12.4G    0.03325    0.01296   0.003221         68        640: 100% 10/10 [00:06<00:00,  1.58it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.41it/s]
                   all        100        196      0.909      0.807      0.873      0.448

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     50/999      12.4G    0.03415    0.01241   0.004985         92        640: 100% 10/10 [00:05<00:00,  1.70it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.55it/s]
                   all        100        196      0.866      0.768      0.811      0.381

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     51/999      12.4G    0.03345    0.01241   0.003808         70        640: 100% 10/10 [00:06<00:00,  1.58it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.51it/s]
                   all        100        196       0.81      0.768      0.823      0.407

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     52/999      12.4G    0.03298    0.01287   0.003346         79        640: 100% 10/10 [00:05<00:00,  1.70it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.54it/s]
                   all        100        196      0.814      0.827      0.807      0.419

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     53/999      12.4G     0.0324    0.01303   0.003554         77        640: 100% 10/10 [00:06<00:00,  1.58it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.53it/s]
                   all        100        196      0.794      0.803        0.8      0.431

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     54/999      12.4G    0.03133    0.01288   0.004287         87        640: 100% 10/10 [00:05<00:00,  1.70it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.55it/s]
                   all        100        196      0.864      0.781      0.861      0.468

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     55/999      12.4G    0.03252    0.01155   0.003892         75        640: 100% 10/10 [00:06<00:00,  1.56it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.53it/s]
                   all        100        196      0.832      0.822      0.862      0.434

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     56/999      12.4G    0.03251    0.01226   0.003563         95        640: 100% 10/10 [00:05<00:00,  1.69it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.54it/s]
                   all        100        196      0.839      0.829      0.852      0.468

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     57/999      12.4G    0.03159    0.01172   0.002947         77        640: 100% 10/10 [00:06<00:00,  1.57it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.52it/s]
                   all        100        196       0.82      0.851      0.868      0.454

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     58/999      12.4G    0.03235    0.01246   0.003773         74        640: 100% 10/10 [00:05<00:00,  1.70it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.54it/s]
                   all        100        196      0.857      0.809      0.868      0.484

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     59/999      12.4G    0.03278    0.01214   0.003574         64        640: 100% 10/10 [00:06<00:00,  1.57it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.54it/s]
                   all        100        196      0.837      0.804       0.82       0.44

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     60/999      12.4G     0.0311    0.01238   0.003743         50        640: 100% 10/10 [00:05<00:00,  1.70it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.56it/s]
                   all        100        196       0.84       0.77       0.83      0.438

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     61/999      12.4G    0.03106    0.01178   0.004169         74        640: 100% 10/10 [00:06<00:00,  1.58it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.54it/s]
                   all        100        196      0.902       0.78       0.85      0.467

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     62/999      12.4G    0.02991    0.01243   0.003425         66        640: 100% 10/10 [00:05<00:00,  1.70it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.37it/s]
                   all        100        196      0.818      0.835      0.857      0.476

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     63/999      12.4G    0.03057    0.01196   0.003537         69        640: 100% 10/10 [00:06<00:00,  1.60it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.54it/s]
                   all        100        196      0.797       0.81      0.847      0.463

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     64/999      12.4G    0.03152    0.01234   0.003626         63        640: 100% 10/10 [00:05<00:00,  1.70it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.33it/s]
                   all        100        196       0.81      0.766      0.819      0.453

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     65/999      12.4G    0.03254    0.01214   0.004204         61        640: 100% 10/10 [00:06<00:00,  1.63it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.55it/s]
                   all        100        196      0.783      0.701       0.74      0.392

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     66/999      12.4G    0.02994    0.01172   0.003327         46        640: 100% 10/10 [00:05<00:00,  1.68it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.33it/s]
                   all        100        196      0.862      0.803      0.868      0.496

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     67/999      12.4G    0.03214    0.01168    0.00321         61        640: 100% 10/10 [00:06<00:00,  1.66it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.55it/s]
                   all        100        196      0.825      0.785      0.836      0.473

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     68/999      12.4G    0.03068    0.01182   0.003008         70        640: 100% 10/10 [00:06<00:00,  1.64it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.34it/s]
                   all        100        196      0.893      0.845      0.886       0.48

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     69/999      12.4G    0.03083    0.01125   0.003549         49        640: 100% 10/10 [00:06<00:00,  1.66it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.53it/s]
                   all        100        196      0.853      0.884      0.907      0.509

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     70/999      12.4G    0.03007    0.01113   0.003989         57        640: 100% 10/10 [00:06<00:00,  1.62it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.30it/s]
                   all        100        196      0.853      0.885      0.899      0.505

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     71/999      12.4G    0.02892    0.01232   0.003066         72        640: 100% 10/10 [00:05<00:00,  1.71it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.54it/s]
                   all        100        196      0.901      0.844      0.891      0.499

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     72/999      12.4G    0.02923     0.0117   0.003117         81        640: 100% 10/10 [00:06<00:00,  1.61it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.27it/s]
                   all        100        196      0.758      0.791      0.839      0.459

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     73/999      12.4G    0.03038     0.0128   0.002919         90        640: 100% 10/10 [00:05<00:00,  1.70it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.55it/s]
                   all        100        196      0.861      0.796      0.841       0.43

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     74/999      12.4G    0.03219    0.01146   0.002775         69        640: 100% 10/10 [00:06<00:00,  1.58it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.36it/s]
                   all        100        196      0.858      0.789       0.87      0.469

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     75/999      12.4G     0.0295    0.01287   0.002962         90        640: 100% 10/10 [00:05<00:00,  1.70it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.54it/s]
                   all        100        196      0.811      0.772      0.821      0.456

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     76/999      12.4G    0.02824    0.01135   0.002902         93        640: 100% 10/10 [00:06<00:00,  1.58it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.47it/s]
                   all        100        196      0.807      0.831      0.858      0.489

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     77/999      12.4G     0.0295    0.01207   0.002432         89        640: 100% 10/10 [00:05<00:00,  1.70it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.55it/s]
                   all        100        196      0.755      0.822      0.841      0.476

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     78/999      12.4G    0.03047    0.01065   0.002873         70        640: 100% 10/10 [00:06<00:00,  1.55it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.54it/s]
                   all        100        196      0.862      0.828      0.868      0.491

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     79/999      12.4G      0.029    0.01189   0.003759         64        640: 100% 10/10 [00:05<00:00,  1.70it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.55it/s]
                   all        100        196      0.809      0.834      0.869      0.465

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     80/999      12.4G    0.03022    0.01145   0.003009         81        640: 100% 10/10 [00:06<00:00,  1.55it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.56it/s]
                   all        100        196      0.809      0.832      0.827      0.419

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     81/999      12.4G    0.02806    0.01082    0.00283         78        640: 100% 10/10 [00:05<00:00,  1.70it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.55it/s]
                   all        100        196      0.777      0.826      0.801      0.438

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     82/999      12.4G    0.02756    0.01105   0.002385         72        640: 100% 10/10 [00:06<00:00,  1.57it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.54it/s]
                   all        100        196      0.879      0.837       0.87      0.506

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     83/999      12.4G    0.02789    0.01096   0.002551         63        640: 100% 10/10 [00:05<00:00,  1.71it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.56it/s]
                   all        100        196      0.908      0.799      0.875      0.497

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     84/999      12.4G    0.02522    0.01054   0.001923         48        640: 100% 10/10 [00:06<00:00,  1.57it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.53it/s]
                   all        100        196      0.852       0.85      0.892      0.496

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     85/999      12.4G    0.02913    0.01073   0.002193         72        640: 100% 10/10 [00:05<00:00,  1.70it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.54it/s]
                   all        100        196      0.873      0.833      0.884      0.485

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     86/999      12.4G    0.02869    0.01125   0.002838         90        640: 100% 10/10 [00:06<00:00,  1.55it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.55it/s]
                   all        100        196      0.859      0.858      0.907      0.523

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     87/999      12.4G    0.02819    0.01152   0.001955         69        640: 100% 10/10 [00:05<00:00,  1.71it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.42it/s]
                   all        100        196      0.906      0.855        0.9      0.503

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     88/999      12.4G     0.0288    0.01065   0.002997         76        640: 100% 10/10 [00:06<00:00,  1.59it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.55it/s]
                   all        100        196      0.931       0.83      0.898      0.499

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     89/999      12.4G    0.02829    0.01088   0.003105         73        640: 100% 10/10 [00:05<00:00,  1.70it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.36it/s]
                   all        100        196      0.935      0.814      0.895        0.5

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     90/999      12.4G    0.02991    0.01091      0.003         74        640: 100% 10/10 [00:06<00:00,  1.63it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.54it/s]
                   all        100        196      0.912       0.81      0.882        0.5

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     91/999      12.4G    0.02807     0.0115    0.00244         66        640: 100% 10/10 [00:05<00:00,  1.69it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.35it/s]
                   all        100        196      0.852      0.868      0.894      0.493

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     92/999      12.4G      0.029    0.01098   0.002171         63        640: 100% 10/10 [00:06<00:00,  1.55it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.55it/s]
                   all        100        196      0.829      0.834      0.866      0.494

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     93/999      12.4G    0.02748    0.01048   0.002288         76        640: 100% 10/10 [00:05<00:00,  1.68it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.32it/s]
                   all        100        196       0.94      0.779      0.898      0.498

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     94/999      12.4G    0.02761    0.01029   0.002451         71        640: 100% 10/10 [00:06<00:00,  1.64it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.54it/s]
                   all        100        196      0.921      0.826      0.898        0.5

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     95/999      12.4G    0.02694    0.01111   0.002576         67        640: 100% 10/10 [00:06<00:00,  1.66it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.30it/s]
                   all        100        196      0.873      0.871      0.909      0.499

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     96/999      12.4G    0.02593   0.009954     0.0024         67        640: 100% 10/10 [00:05<00:00,  1.67it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.53it/s]
                   all        100        196      0.882        0.8      0.887      0.508

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     97/999      12.4G    0.02588    0.01017   0.002613         63        640: 100% 10/10 [00:06<00:00,  1.65it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.35it/s]
                   all        100        196      0.893      0.807      0.879      0.494

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     98/999      12.4G    0.02587    0.01021   0.002779         62        640: 100% 10/10 [00:05<00:00,  1.68it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.54it/s]
                   all        100        196      0.916      0.808      0.888      0.498

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
     99/999      12.4G    0.02845    0.01045   0.002273         70        640: 100% 10/10 [00:06<00:00,  1.63it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.36it/s]
                   all        100        196      0.929      0.801       0.89        0.5

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    100/999      12.4G    0.02732    0.01041   0.002906         72        640: 100% 10/10 [00:05<00:00,  1.70it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.55it/s]
                   all        100        196      0.906      0.798      0.881      0.488

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    101/999      12.4G    0.02598    0.01021   0.003473         65        640: 100% 10/10 [00:06<00:00,  1.62it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.34it/s]
                   all        100        196      0.905       0.79      0.876      0.491

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    102/999      12.4G    0.02628    0.01078   0.002752         92        640: 100% 10/10 [00:05<00:00,  1.69it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.55it/s]
                   all        100        196      0.915      0.797      0.885      0.496

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    103/999      12.4G    0.02538    0.01035    0.00172         86        640: 100% 10/10 [00:06<00:00,  1.59it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.39it/s]
                   all        100        196      0.824      0.791      0.843      0.476

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    104/999      12.4G    0.02688    0.01051   0.002754         59        640: 100% 10/10 [00:05<00:00,  1.69it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.53it/s]
                   all        100        196      0.864      0.766       0.84      0.466

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    105/999      12.4G    0.02699    0.01018   0.002499         63        640: 100% 10/10 [00:06<00:00,  1.60it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.49it/s]
                   all        100        196      0.865      0.821      0.856      0.477

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    106/999      12.4G    0.02503    0.01092   0.002241         67        640: 100% 10/10 [00:05<00:00,  1.70it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.55it/s]
                   all        100        196      0.884      0.783      0.851      0.455

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    107/999      12.4G    0.02569     0.0112   0.002541         97        640: 100% 10/10 [00:06<00:00,  1.56it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.57it/s]
                   all        100        196      0.896      0.861      0.908       0.49

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    108/999      12.4G    0.02607   0.009798   0.002644         75        640: 100% 10/10 [00:05<00:00,  1.70it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.56it/s]
                   all        100        196      0.899       0.83      0.898      0.482

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    109/999      12.4G    0.02527   0.009976    0.00244         67        640: 100% 10/10 [00:06<00:00,  1.58it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.54it/s]
                   all        100        196      0.853      0.848      0.882      0.488

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    110/999      12.4G    0.02582    0.01098   0.002658         82        640: 100% 10/10 [00:05<00:00,  1.70it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.56it/s]
                   all        100        196       0.84      0.861      0.877      0.467

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    111/999      12.4G    0.02565    0.01031    0.00197         68        640: 100% 10/10 [00:06<00:00,  1.58it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.55it/s]
                   all        100        196      0.903      0.799      0.872      0.492

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    112/999      12.4G    0.02603    0.01001   0.002278         61        640: 100% 10/10 [00:05<00:00,  1.69it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.55it/s]
                   all        100        196      0.851      0.842      0.877      0.471

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    113/999      12.4G    0.02622    0.01072   0.002471         87        640: 100% 10/10 [00:06<00:00,  1.55it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.55it/s]
                   all        100        196      0.901      0.835      0.891      0.492

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    114/999      12.4G    0.02605     0.0108    0.00235         56        640: 100% 10/10 [00:05<00:00,  1.70it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.54it/s]
                   all        100        196      0.908       0.82      0.887      0.502

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    115/999      12.4G    0.02484    0.01014   0.002161         79        640: 100% 10/10 [00:06<00:00,  1.56it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.55it/s]
                   all        100        196      0.878      0.828      0.879      0.479

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    116/999      12.4G    0.02737    0.01076   0.002082         70        640: 100% 10/10 [00:05<00:00,  1.69it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.56it/s]
                   all        100        196      0.908      0.813      0.854      0.502

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    117/999      12.4G    0.02481   0.009575   0.002193         60        640: 100% 10/10 [00:06<00:00,  1.58it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.57it/s]
                   all        100        196      0.906      0.836      0.878      0.504

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    118/999      12.4G    0.02433    0.01095   0.001962         76        640: 100% 10/10 [00:05<00:00,  1.69it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.45it/s]
                   all        100        196      0.913      0.831      0.873      0.509

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    119/999      12.4G     0.0256     0.0091   0.001668         65        640: 100% 10/10 [00:06<00:00,  1.59it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.52it/s]
                   all        100        196      0.945      0.821      0.879      0.496

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    120/999      12.4G    0.02413   0.009379   0.001805         75        640: 100% 10/10 [00:05<00:00,  1.70it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.42it/s]
                   all        100        196      0.878      0.784       0.84      0.482

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    121/999      12.4G    0.02478   0.009886   0.001802         93        640: 100% 10/10 [00:06<00:00,  1.59it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.56it/s]
                   all        100        196      0.864      0.826      0.832       0.48

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    122/999      12.4G    0.02498    0.01009   0.002395         64        640: 100% 10/10 [00:05<00:00,  1.69it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.35it/s]
                   all        100        196      0.861      0.844      0.848      0.503

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    123/999      12.4G    0.02412   0.009523    0.00229         76        640: 100% 10/10 [00:06<00:00,  1.60it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.55it/s]
                   all        100        196      0.865      0.845      0.873      0.508

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    124/999      12.4G    0.02389   0.009772   0.002079         60        640: 100% 10/10 [00:05<00:00,  1.69it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.37it/s]
                   all        100        196      0.917      0.809      0.879      0.512

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    125/999      12.4G     0.0257    0.01038   0.002798         81        640: 100% 10/10 [00:06<00:00,  1.63it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.51it/s]
                   all        100        196      0.851      0.862      0.882      0.512

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    126/999      12.4G    0.02402    0.01033    0.00212         57        640: 100% 10/10 [00:05<00:00,  1.67it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.35it/s]
                   all        100        196      0.849      0.833      0.888      0.518

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    127/999      12.4G    0.02341     0.0101   0.002031         78        640: 100% 10/10 [00:06<00:00,  1.63it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.59it/s]
                   all        100        196       0.85      0.808      0.867      0.505

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    128/999      12.4G    0.02721    0.01007   0.002294         70        640: 100% 10/10 [00:05<00:00,  1.67it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.28it/s]
                   all        100        196      0.889      0.774      0.845        0.5

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    129/999      12.4G    0.02395     0.0104   0.001797         71        640: 100% 10/10 [00:06<00:00,  1.67it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.53it/s]
                   all        100        196      0.868      0.774      0.822      0.485

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    130/999      12.4G    0.02475   0.009057   0.001526         67        640: 100% 10/10 [00:06<00:00,  1.65it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.29it/s]
                   all        100        196      0.889      0.791      0.846      0.484

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    131/999      12.4G    0.02279   0.009661   0.001674         74        640: 100% 10/10 [00:06<00:00,  1.66it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.55it/s]
                   all        100        196      0.922      0.793      0.871      0.509

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    132/999      12.4G    0.02418    0.00859   0.001457         58        640: 100% 10/10 [00:06<00:00,  1.63it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.35it/s]
                   all        100        196      0.916      0.813      0.872      0.516

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    133/999      12.4G    0.02257   0.009362   0.001988         50        640: 100% 10/10 [00:05<00:00,  1.71it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.54it/s]
                   all        100        196      0.901      0.841      0.885      0.517

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    134/999      12.4G    0.02375   0.009507   0.001996         72        640: 100% 10/10 [00:06<00:00,  1.61it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.29it/s]
                   all        100        196      0.908      0.839      0.888      0.525

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    135/999      12.4G    0.02166    0.00913   0.002363         65        640: 100% 10/10 [00:05<00:00,  1.69it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.53it/s]
                   all        100        196      0.872       0.85      0.885      0.518

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    136/999      12.4G    0.02331   0.009435   0.001652         80        640: 100% 10/10 [00:06<00:00,  1.56it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.35it/s]
                   all        100        196      0.904      0.817      0.858      0.497

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    137/999      12.4G    0.02485   0.009662   0.001608         60        640: 100% 10/10 [00:05<00:00,  1.70it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.55it/s]
                   all        100        196      0.902      0.798      0.852      0.499

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    138/999      12.4G    0.02202   0.009533   0.001477         77        640: 100% 10/10 [00:06<00:00,  1.58it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.36it/s]
                   all        100        196      0.863      0.821      0.865      0.492

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    139/999      12.4G     0.0232   0.009066   0.001759         63        640: 100% 10/10 [00:05<00:00,  1.69it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.55it/s]
                   all        100        196      0.836      0.851      0.862      0.479

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    140/999      12.4G    0.02404    0.00883   0.001697         76        640: 100% 10/10 [00:06<00:00,  1.58it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.39it/s]
                   all        100        196      0.891      0.761      0.846      0.475

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    141/999      12.4G    0.02362   0.009948   0.002074         83        640: 100% 10/10 [00:05<00:00,  1.69it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.54it/s]
                   all        100        196      0.885      0.819      0.864      0.495

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    142/999      12.4G    0.02397   0.009673   0.001676         70        640: 100% 10/10 [00:06<00:00,  1.58it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.54it/s]
                   all        100        196       0.89      0.806      0.867      0.519

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    143/999      12.4G    0.02401   0.009339   0.001516         63        640: 100% 10/10 [00:05<00:00,  1.68it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.53it/s]
                   all        100        196      0.913      0.797      0.864      0.512

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    144/999      12.4G    0.02163    0.00945   0.002228         66        640: 100% 10/10 [00:06<00:00,  1.57it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.55it/s]
                   all        100        196      0.911      0.822      0.868      0.505

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    145/999      12.4G    0.02327   0.009173   0.001374         70        640: 100% 10/10 [00:05<00:00,  1.70it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.55it/s]
                   all        100        196      0.904      0.811      0.874      0.494

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    146/999      12.4G     0.0244   0.009745   0.001763         79        640: 100% 10/10 [00:06<00:00,  1.57it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.56it/s]
                   all        100        196      0.847      0.823      0.849      0.492

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    147/999      12.4G    0.02366   0.009796   0.001677         75        640: 100% 10/10 [00:05<00:00,  1.69it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.53it/s]
                   all        100        196      0.842      0.846      0.856      0.509

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    148/999      12.4G    0.02276    0.01044   0.001894         76        640: 100% 10/10 [00:06<00:00,  1.55it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.55it/s]
                   all        100        196      0.874      0.855       0.89      0.525

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    149/999      12.4G    0.02226   0.009194   0.002349         83        640: 100% 10/10 [00:05<00:00,  1.68it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.48it/s]
                   all        100        196      0.906      0.843      0.885      0.511

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    150/999      12.4G    0.02325   0.009775   0.002621         94        640: 100% 10/10 [00:06<00:00,  1.61it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.56it/s]
                   all        100        196      0.927      0.793      0.879       0.49

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    151/999      12.4G    0.02294   0.009382   0.001322         75        640: 100% 10/10 [00:05<00:00,  1.70it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.46it/s]
                   all        100        196      0.955      0.799      0.884      0.505

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    152/999      12.4G    0.02353   0.009537   0.001477         76        640: 100% 10/10 [00:06<00:00,  1.60it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.55it/s]
                   all        100        196      0.933      0.826       0.87       0.52

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    153/999      12.4G    0.02242   0.008789   0.001694         79        640: 100% 10/10 [00:05<00:00,  1.70it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.38it/s]
                   all        100        196      0.923      0.819      0.877      0.534

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    154/999      12.4G    0.02174   0.009567   0.002124         70        640: 100% 10/10 [00:06<00:00,  1.60it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.56it/s]
                   all        100        196      0.928      0.796      0.863      0.514

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    155/999      12.4G    0.02435   0.009649   0.001934         60        640: 100% 10/10 [00:05<00:00,  1.67it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.35it/s]
                   all        100        196      0.913      0.783      0.857      0.501

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    156/999      12.4G    0.02101   0.009393   0.001643         66        640: 100% 10/10 [00:06<00:00,  1.61it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.53it/s]
                   all        100        196      0.902      0.786       0.87      0.518

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    157/999      12.4G    0.02214   0.008791   0.001955         73        640: 100% 10/10 [00:06<00:00,  1.64it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.27it/s]
                   all        100        196      0.828      0.851       0.86      0.501

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    158/999      12.4G     0.0221   0.009429   0.002396         70        640: 100% 10/10 [00:06<00:00,  1.65it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.54it/s]
                   all        100        196      0.903      0.796      0.861      0.489

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    159/999      12.4G    0.02208    0.00883   0.001854         60        640: 100% 10/10 [00:06<00:00,  1.60it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.27it/s]
                   all        100        196      0.891      0.812      0.866      0.509

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    160/999      12.4G    0.02284   0.009335   0.001511         71        640: 100% 10/10 [00:05<00:00,  1.68it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.52it/s]
                   all        100        196      0.868      0.832      0.873      0.499

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    161/999      12.4G    0.02316   0.009234    0.00161         60        640: 100% 10/10 [00:06<00:00,  1.59it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.30it/s]
                   all        100        196      0.899      0.832      0.907      0.521

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    162/999      12.4G    0.02079   0.008694   0.002004         62        640: 100% 10/10 [00:05<00:00,  1.69it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.51it/s]
                   all        100        196      0.898       0.85      0.901      0.525

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    163/999      12.4G    0.02264   0.008766    0.00151         80        640: 100% 10/10 [00:06<00:00,  1.60it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.38it/s]
                   all        100        196      0.923      0.806      0.882       0.49

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    164/999      12.4G    0.02263   0.009556   0.001445         68        640: 100% 10/10 [00:05<00:00,  1.69it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.53it/s]
                   all        100        196      0.927      0.813      0.887      0.515

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    165/999      12.4G    0.02084   0.009103   0.001798         77        640: 100% 10/10 [00:06<00:00,  1.56it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.45it/s]
                   all        100        196      0.896      0.815      0.889      0.515

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    166/999      12.4G    0.02142   0.009229    0.00126         75        640: 100% 10/10 [00:05<00:00,  1.70it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.53it/s]
                   all        100        196       0.88      0.846      0.892       0.52

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    167/999      12.4G    0.02017   0.009055   0.001356         84        640: 100% 10/10 [00:06<00:00,  1.58it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.53it/s]
                   all        100        196      0.924      0.844      0.901      0.537

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    168/999      12.4G    0.02174   0.008623   0.001736         60        640: 100% 10/10 [00:05<00:00,  1.69it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.56it/s]
                   all        100        196      0.913      0.845      0.896      0.527

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    169/999      12.4G    0.02224   0.009298   0.001843         74        640: 100% 10/10 [00:06<00:00,  1.57it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.53it/s]
                   all        100        196      0.901      0.862      0.898      0.528

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    170/999      12.4G    0.02137   0.008515   0.001941         81        640: 100% 10/10 [00:05<00:00,  1.69it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.57it/s]
                   all        100        196      0.901      0.839      0.895        0.5

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    171/999      12.4G    0.02156   0.008247   0.001573         61        640: 100% 10/10 [00:06<00:00,  1.55it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.54it/s]
                   all        100        196      0.913      0.824      0.892      0.508

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    172/999      12.4G    0.02071   0.008333   0.001912         65        640: 100% 10/10 [00:05<00:00,  1.69it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.52it/s]
                   all        100        196      0.845      0.857      0.875      0.512

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    173/999      12.4G    0.02031   0.008647    0.00152         79        640: 100% 10/10 [00:06<00:00,  1.56it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.56it/s]
                   all        100        196      0.864      0.808      0.842      0.497

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    174/999      12.4G    0.02038   0.008895   0.001809         66        640: 100% 10/10 [00:05<00:00,  1.68it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.49it/s]
                   all        100        196      0.893      0.777      0.859      0.532

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    175/999      12.4G     0.0213   0.009313   0.001251         67        640: 100% 10/10 [00:06<00:00,  1.59it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.55it/s]
                   all        100        196      0.917      0.795      0.876      0.533

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    176/999      12.4G     0.0202   0.007758   0.001168         59        640: 100% 10/10 [00:05<00:00,  1.69it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.45it/s]
                   all        100        196      0.862      0.853      0.888       0.53

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    177/999      12.4G    0.02136    0.00799    0.00108         53        640: 100% 10/10 [00:06<00:00,  1.60it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.54it/s]
                   all        100        196      0.909      0.834      0.884      0.517

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    178/999      12.4G    0.02169   0.008879   0.001237         63        640: 100% 10/10 [00:05<00:00,  1.68it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.47it/s]
                   all        100        196      0.934      0.807      0.882      0.533

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    179/999      12.4G    0.02099   0.008218    0.00132         67        640: 100% 10/10 [00:06<00:00,  1.59it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.55it/s]
                   all        100        196      0.933      0.831      0.886      0.539

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    180/999      12.4G    0.02046   0.008587   0.001704         64        640: 100% 10/10 [00:05<00:00,  1.69it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.35it/s]
                   all        100        196      0.916      0.841      0.901      0.524

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    181/999      12.4G    0.02117   0.008989   0.001135         82        640: 100% 10/10 [00:06<00:00,  1.53it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.56it/s]
                   all        100        196      0.921      0.824      0.886      0.515

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    182/999      12.4G    0.01889   0.008651   0.001541         64        640: 100% 10/10 [00:05<00:00,  1.69it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.32it/s]
                   all        100        196      0.927      0.809      0.865      0.508

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    183/999      12.4G    0.02119   0.008256    0.00153         65        640: 100% 10/10 [00:06<00:00,  1.62it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.55it/s]
                   all        100        196      0.898      0.823       0.86      0.506

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    184/999      12.4G    0.02023   0.008786   0.001715         54        640: 100% 10/10 [00:06<00:00,  1.66it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.33it/s]
                   all        100        196      0.866      0.834      0.864      0.501

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    185/999      12.4G     0.0214    0.00916   0.002021        102        640: 100% 10/10 [00:06<00:00,  1.64it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.56it/s]
                   all        100        196      0.902      0.851      0.878      0.517

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    186/999      12.4G    0.02028   0.007715   0.001082         76        640: 100% 10/10 [00:06<00:00,  1.64it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.32it/s]
                   all        100        196      0.919       0.84      0.894      0.518

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    187/999      12.4G    0.02127   0.008336   0.001507         58        640: 100% 10/10 [00:06<00:00,  1.67it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.55it/s]
                   all        100        196      0.894      0.869      0.897      0.522

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    188/999      12.4G    0.01883    0.00837   0.001034         60        640: 100% 10/10 [00:06<00:00,  1.63it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.31it/s]
                   all        100        196       0.94      0.831      0.896      0.522

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    189/999      12.4G    0.02176   0.008356   0.001869         66        640: 100% 10/10 [00:05<00:00,  1.69it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.54it/s]
                   all        100        196       0.91      0.843        0.9      0.519

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    190/999      12.4G    0.02107    0.00842   0.001641         54        640: 100% 10/10 [00:06<00:00,  1.60it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.28it/s]
                   all        100        196      0.882      0.841      0.888      0.526

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    191/999      12.4G    0.02055   0.008014   0.001227         51        640: 100% 10/10 [00:05<00:00,  1.69it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.56it/s]
                   all        100        196      0.871      0.821      0.875      0.507

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    192/999      12.4G    0.01933   0.008721   0.001307         59        640: 100% 10/10 [00:06<00:00,  1.58it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.38it/s]
                   all        100        196      0.919       0.78      0.858      0.515

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    193/999      12.4G    0.02146   0.008941   0.001993         89        640: 100% 10/10 [00:05<00:00,  1.67it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.56it/s]
                   all        100        196      0.933      0.795       0.86       0.52

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    194/999      12.4G    0.01964   0.008745   0.001607         93        640: 100% 10/10 [00:06<00:00,  1.57it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.42it/s]
                   all        100        196      0.929      0.825      0.875      0.521

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    195/999      12.4G    0.02068   0.008794   0.002107         75        640: 100% 10/10 [00:05<00:00,  1.68it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.53it/s]
                   all        100        196      0.871      0.844       0.89      0.513

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    196/999      12.4G    0.02037   0.007604   0.001599         44        640: 100% 10/10 [00:06<00:00,  1.59it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.55it/s]
                   all        100        196      0.893      0.826      0.879      0.517

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    197/999      12.4G    0.02025   0.008468   0.001546         75        640: 100% 10/10 [00:06<00:00,  1.62it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.57it/s]
                   all        100        196      0.852      0.793      0.851      0.504

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    198/999      12.4G    0.01983   0.008449   0.001452         68        640: 100% 10/10 [00:06<00:00,  1.55it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.55it/s]
                   all        100        196      0.824      0.785      0.841      0.487

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    199/999      12.4G    0.02017   0.008896   0.001317         97        640: 100% 10/10 [00:05<00:00,  1.68it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.56it/s]
                   all        100        196      0.827      0.807      0.848      0.485

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    200/999      12.4G    0.01987   0.008723   0.001867         77        640: 100% 10/10 [00:06<00:00,  1.58it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.57it/s]
                   all        100        196       0.85      0.799      0.855      0.489

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    201/999      12.4G    0.01992   0.007721   0.002867         73        640: 100% 10/10 [00:05<00:00,  1.70it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.53it/s]
                   all        100        196      0.877       0.76       0.84      0.491

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    202/999      12.4G    0.01973   0.008485   0.001538         81        640: 100% 10/10 [00:06<00:00,  1.58it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.54it/s]
                   all        100        196        0.9      0.788      0.869      0.513

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    203/999      12.4G    0.01947   0.007283   0.001706         69        640: 100% 10/10 [00:05<00:00,  1.70it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.54it/s]
                   all        100        196      0.932      0.816      0.896      0.508

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    204/999      12.4G    0.01921   0.008202   0.001912         61        640: 100% 10/10 [00:06<00:00,  1.57it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.54it/s]
                   all        100        196      0.859       0.86      0.882      0.505

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    205/999      12.4G    0.02018    0.00903   0.001458         62        640: 100% 10/10 [00:05<00:00,  1.69it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.54it/s]
                   all        100        196      0.904      0.823      0.905      0.514

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    206/999      12.4G     0.0192   0.007829   0.001593         53        640: 100% 10/10 [00:06<00:00,  1.58it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.53it/s]
                   all        100        196      0.891      0.844      0.892      0.522

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    207/999      12.4G    0.02032   0.008398    0.00168         71        640: 100% 10/10 [00:05<00:00,  1.70it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.53it/s]
                   all        100        196      0.891      0.844      0.898      0.527

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    208/999      12.4G    0.02111    0.00893   0.001783         90        640: 100% 10/10 [00:06<00:00,  1.55it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.56it/s]
                   all        100        196      0.924      0.768      0.846      0.495

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    209/999      12.4G    0.01963   0.008261   0.001191         66        640: 100% 10/10 [00:05<00:00,  1.69it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.55it/s]
                   all        100        196       0.95      0.781      0.853      0.502

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    210/999      12.4G    0.02013   0.007916   0.001749         64        640: 100% 10/10 [00:06<00:00,  1.55it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.53it/s]
                   all        100        196      0.939      0.769      0.866      0.507

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    211/999      12.4G    0.01945   0.008611   0.001342         75        640: 100% 10/10 [00:05<00:00,  1.67it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.57it/s]
                   all        100        196      0.896      0.782      0.874      0.512

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    212/999      12.4G    0.01976   0.008037   0.001468         69        640: 100% 10/10 [00:06<00:00,  1.58it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.54it/s]
                   all        100        196      0.857      0.792       0.86        0.5

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    213/999      12.4G    0.01927   0.007674   0.001465         77        640: 100% 10/10 [00:06<00:00,  1.63it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.53it/s]
                   all        100        196      0.887      0.808      0.855      0.494

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    214/999      12.4G    0.01903   0.008075   0.001404         74        640: 100% 10/10 [00:06<00:00,  1.55it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.56it/s]
                   all        100        196      0.965      0.779      0.876      0.503

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    215/999      12.4G    0.01934   0.008647    0.00125         59        640: 100% 10/10 [00:05<00:00,  1.68it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.54it/s]
                   all        100        196       0.94        0.8      0.885      0.512

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    216/999      12.4G    0.01986   0.008459   0.001552         77        640: 100% 10/10 [00:06<00:00,  1.59it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.56it/s]
                   all        100        196      0.897       0.84      0.888      0.511

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    217/999      12.4G    0.01846    0.00891    0.00116         64        640: 100% 10/10 [00:05<00:00,  1.70it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.45it/s]
                   all        100        196      0.911      0.822      0.885      0.516

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    218/999      12.4G    0.01848   0.008174   0.001164         69        640: 100% 10/10 [00:06<00:00,  1.61it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.56it/s]
                   all        100        196      0.902      0.798      0.887      0.521

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    219/999      12.4G    0.01899   0.008789   0.001767         98        640: 100% 10/10 [00:05<00:00,  1.68it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.41it/s]
                   all        100        196       0.94      0.801      0.902      0.523

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    220/999      12.4G    0.01829   0.009103   0.001189         83        640: 100% 10/10 [00:06<00:00,  1.60it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.54it/s]
                   all        100        196       0.89      0.844      0.897      0.523

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    221/999      12.4G    0.01865   0.007656   0.001427         62        640: 100% 10/10 [00:05<00:00,  1.69it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.35it/s]
                   all        100        196      0.884      0.848      0.885      0.528

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    222/999      12.4G    0.01863   0.008111   0.001319         50        640: 100% 10/10 [00:06<00:00,  1.64it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.55it/s]
                   all        100        196      0.911      0.849      0.889      0.517

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    223/999      12.4G    0.01953   0.008266   0.001662         76        640: 100% 10/10 [00:05<00:00,  1.67it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.32it/s]
                   all        100        196      0.906       0.83      0.881       0.51

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    224/999      12.4G    0.02102   0.009152   0.001198         97        640: 100% 10/10 [00:06<00:00,  1.63it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.56it/s]
                   all        100        196        0.9      0.838      0.888       0.52

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    225/999      12.4G    0.01845   0.008107   0.001611         77        640: 100% 10/10 [00:06<00:00,  1.66it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.34it/s]
                   all        100        196      0.941      0.802      0.877      0.524

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    226/999      12.4G    0.01801   0.008046   0.001339         86        640: 100% 10/10 [00:06<00:00,  1.66it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.56it/s]
                   all        100        196      0.957      0.805      0.898      0.533

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    227/999      12.4G    0.01907   0.008417   0.001108         68        640: 100% 10/10 [00:05<00:00,  1.67it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.28it/s]
                   all        100        196      0.917      0.841       0.89      0.534

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    228/999      12.4G    0.01966      0.008   0.001236         83        640: 100% 10/10 [00:06<00:00,  1.65it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.52it/s]
                   all        100        196       0.91      0.848      0.891       0.54

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    229/999      12.4G    0.01819   0.007574   0.001408         65        640: 100% 10/10 [00:06<00:00,  1.62it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.33it/s]
                   all        100        196      0.853      0.861      0.882      0.532

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    230/999      12.4G    0.01867    0.00844   0.001693         86        640: 100% 10/10 [00:05<00:00,  1.69it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.54it/s]
                   all        100        196      0.821      0.843      0.878      0.511

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    231/999      12.4G     0.0192   0.008089   0.001662         75        640: 100% 10/10 [00:06<00:00,  1.61it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.27it/s]
                   all        100        196      0.899      0.792      0.876      0.506

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    232/999      12.4G    0.01799    0.00728   0.001342         41        640: 100% 10/10 [00:05<00:00,  1.67it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.54it/s]
                   all        100        196      0.866      0.824      0.877      0.514

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    233/999      12.4G    0.01747   0.007924   0.001396         66        640: 100% 10/10 [00:06<00:00,  1.60it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.34it/s]
                   all        100        196      0.848      0.856      0.889      0.525

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    234/999      12.4G    0.01828   0.007991   0.001308         59        640: 100% 10/10 [00:05<00:00,  1.70it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.54it/s]
                   all        100        196      0.897      0.818      0.888      0.516

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    235/999      12.4G    0.01807   0.007833   0.001049         56        640: 100% 10/10 [00:06<00:00,  1.59it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.33it/s]
                   all        100        196      0.923      0.796      0.878      0.521

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    236/999      12.4G    0.01726   0.007408   0.001409         69        640: 100% 10/10 [00:05<00:00,  1.69it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.56it/s]
                   all        100        196      0.937      0.808      0.887      0.518

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    237/999      12.4G     0.0176   0.007891     0.0013         63        640: 100% 10/10 [00:06<00:00,  1.55it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.55it/s]
                   all        100        196      0.894      0.843      0.881      0.512

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    238/999      12.4G    0.01805   0.008465   0.001147         58        640: 100% 10/10 [00:05<00:00,  1.68it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.57it/s]
                   all        100        196       0.89      0.858      0.894      0.513

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    239/999      12.4G    0.01828   0.007965   0.001478         65        640: 100% 10/10 [00:06<00:00,  1.57it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.53it/s]
                   all        100        196      0.875      0.853      0.884      0.514

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    240/999      12.4G    0.01882   0.008123   0.001197         92        640: 100% 10/10 [00:05<00:00,  1.68it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.56it/s]
                   all        100        196       0.92      0.839      0.899      0.526

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    241/999      12.4G    0.01798   0.007619   0.001531         63        640: 100% 10/10 [00:06<00:00,  1.58it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.56it/s]
                   all        100        196      0.927      0.822      0.892      0.529

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    242/999      12.4G    0.01755    0.00745   0.001341         65        640: 100% 10/10 [00:05<00:00,  1.68it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.56it/s]
                   all        100        196      0.908       0.87      0.911      0.536

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    243/999      12.4G    0.01756   0.007576   0.001806         69        640: 100% 10/10 [00:06<00:00,  1.56it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.52it/s]
                   all        100        196      0.888      0.863      0.904      0.524

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    244/999      12.4G    0.01872   0.008395   0.001479         64        640: 100% 10/10 [00:05<00:00,  1.68it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.54it/s]
                   all        100        196      0.884      0.851      0.892      0.519

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    245/999      12.4G    0.01793   0.007274   0.001119         72        640: 100% 10/10 [00:06<00:00,  1.56it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.56it/s]
                   all        100        196      0.936      0.811      0.887      0.531

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    246/999      12.4G     0.0173   0.008128   0.001158         64        640: 100% 10/10 [00:05<00:00,  1.69it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.55it/s]
                   all        100        196      0.928      0.838      0.885      0.534

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    247/999      12.4G    0.01819   0.007239   0.001442         64        640: 100% 10/10 [00:06<00:00,  1.57it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.55it/s]
                   all        100        196      0.952       0.79      0.874       0.53

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    248/999      12.4G    0.01723    0.00762   0.001287         57        640: 100% 10/10 [00:05<00:00,  1.69it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.56it/s]
                   all        100        196      0.929      0.817      0.866      0.528

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    249/999      12.4G    0.01726   0.008312   0.001193         73        640: 100% 10/10 [00:06<00:00,  1.56it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.55it/s]
                   all        100        196      0.877      0.837      0.868      0.527

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    250/999      12.4G    0.01754    0.00764  0.0009958         57        640: 100% 10/10 [00:05<00:00,  1.69it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.51it/s]
                   all        100        196      0.899      0.825      0.855      0.523

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    251/999      12.4G    0.01882   0.007181    0.00117         55        640: 100% 10/10 [00:06<00:00,  1.56it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.54it/s]
                   all        100        196      0.903      0.833      0.864      0.517

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    252/999      12.4G    0.01727   0.007285   0.001066         66        640: 100% 10/10 [00:05<00:00,  1.70it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.49it/s]
                   all        100        196      0.908      0.805      0.864      0.509

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    253/999      12.4G    0.01701   0.007771  0.0009914         53        640: 100% 10/10 [00:06<00:00,  1.58it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.56it/s]
                   all        100        196      0.901      0.808      0.865      0.517

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    254/999      12.4G    0.01739   0.007956   0.001477         79        640: 100% 10/10 [00:05<00:00,  1.69it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.34it/s]
                   all        100        196      0.933      0.795      0.885      0.525

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    255/999      12.4G    0.01673   0.007756   0.001261         65        640: 100% 10/10 [00:06<00:00,  1.62it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.54it/s]
                   all        100        196      0.942      0.793      0.871      0.524

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    256/999      12.4G    0.01686   0.007204  0.0008614         61        640: 100% 10/10 [00:05<00:00,  1.69it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.36it/s]
                   all        100        196      0.944      0.793      0.879      0.522

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    257/999      12.4G    0.01655   0.007344   0.001211         50        640: 100% 10/10 [00:06<00:00,  1.63it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.53it/s]
                   all        100        196      0.927      0.812      0.886       0.53

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    258/999      12.4G    0.01735   0.007891   0.001388         91        640: 100% 10/10 [00:05<00:00,  1.67it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.34it/s]
                   all        100        196      0.962       0.78      0.898      0.527

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    259/999      12.4G    0.01792   0.007339   0.001325         53        640: 100% 10/10 [00:06<00:00,  1.64it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.54it/s]
                   all        100        196      0.893      0.846        0.9       0.53

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    260/999      12.4G    0.01815   0.008052  0.0009626         75        640: 100% 10/10 [00:06<00:00,  1.65it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.37it/s]
                   all        100        196      0.931      0.808      0.885       0.52

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    261/999      12.4G    0.01881   0.007791   0.001102         55        640: 100% 10/10 [00:06<00:00,  1.63it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.56it/s]
                   all        100        196      0.873      0.815      0.866      0.507

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    262/999      12.4G    0.01793   0.007941   0.001321         81        640: 100% 10/10 [00:06<00:00,  1.64it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.26it/s]
                   all        100        196       0.87       0.83      0.885      0.527

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    263/999      12.4G     0.0182   0.007319   0.001793         83        640: 100% 10/10 [00:05<00:00,  1.67it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.54it/s]
                   all        100        196      0.914      0.795      0.892      0.537

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    264/999      12.4G    0.01735   0.007622   0.001012         63        640: 100% 10/10 [00:06<00:00,  1.60it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.31it/s]
                   all        100        196      0.899       0.85      0.896      0.532

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    265/999      12.4G    0.01666   0.007403  0.0008411         62        640: 100% 10/10 [00:05<00:00,  1.68it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.55it/s]
                   all        100        196      0.899      0.829      0.874       0.52

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    266/999      12.4G    0.01635   0.007792   0.001547         76        640: 100% 10/10 [00:06<00:00,  1.61it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.28it/s]
                   all        100        196       0.95      0.776      0.874      0.509

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    267/999      12.4G    0.01707   0.007667   0.001023         54        640: 100% 10/10 [00:05<00:00,  1.68it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.57it/s]
                   all        100        196      0.928      0.795       0.86       0.51

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    268/999      12.4G    0.01707   0.008249   0.001055         94        640: 100% 10/10 [00:06<00:00,  1.59it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.39it/s]
                   all        100        196      0.943      0.793      0.881      0.516

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    269/999      12.4G    0.01807   0.007457   0.001031         81        640: 100% 10/10 [00:05<00:00,  1.71it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.55it/s]
                   all        100        196      0.895       0.83      0.883      0.526

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    270/999      12.4G    0.01645   0.007451   0.001363         68        640: 100% 10/10 [00:06<00:00,  1.58it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.43it/s]
                   all        100        196      0.935      0.792      0.885      0.521

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    271/999      12.4G    0.01725   0.008016   0.001058         58        640: 100% 10/10 [00:05<00:00,  1.69it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.56it/s]
                   all        100        196      0.872       0.84      0.878      0.528

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    272/999      12.4G      0.018   0.007493  0.0009862         66        640: 100% 10/10 [00:06<00:00,  1.58it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.54it/s]
                   all        100        196      0.907      0.791      0.864      0.518

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    273/999      12.4G    0.01607   0.006685   0.001052         68        640: 100% 10/10 [00:05<00:00,  1.69it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.53it/s]
                   all        100        196      0.876      0.826      0.855      0.517

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    274/999      12.4G    0.01715    0.00767   0.001155         65        640: 100% 10/10 [00:06<00:00,  1.56it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.57it/s]
                   all        100        196       0.86      0.829      0.859      0.523

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    275/999      12.4G    0.01737   0.007112  0.0009864         63        640: 100% 10/10 [00:05<00:00,  1.69it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.56it/s]
                   all        100        196      0.869      0.849      0.865      0.514

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    276/999      12.4G    0.01812   0.007428   0.001335         71        640: 100% 10/10 [00:06<00:00,  1.58it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.53it/s]
                   all        100        196      0.871      0.823      0.867       0.52

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    277/999      12.4G    0.01837   0.007864   0.001604         64        640: 100% 10/10 [00:05<00:00,  1.69it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.56it/s]
                   all        100        196      0.896      0.772      0.849      0.508

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    278/999      12.4G    0.01719   0.007636   0.001229         53        640: 100% 10/10 [00:06<00:00,  1.56it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.56it/s]
                   all        100        196      0.839      0.839      0.875       0.52

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    279/999      12.4G     0.0166   0.007175   0.001025         72        640: 100% 10/10 [00:05<00:00,  1.69it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.56it/s]
                   all        100        196      0.887      0.818      0.882      0.525

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    280/999      12.4G    0.01691   0.006744  0.0007919         79        640: 100% 10/10 [00:06<00:00,  1.55it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.54it/s]
                   all        100        196      0.867      0.842      0.876       0.51

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    281/999      12.4G    0.01607   0.007512   0.001545         68        640: 100% 10/10 [00:05<00:00,  1.70it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.55it/s]
                   all        100        196      0.878      0.816      0.875      0.515

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    282/999      12.4G    0.01644   0.006659   0.001137         83        640: 100% 10/10 [00:06<00:00,  1.53it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.57it/s]
                   all        100        196      0.876      0.819      0.873      0.513

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    283/999      12.4G    0.01787   0.006738   0.001374         52        640: 100% 10/10 [00:05<00:00,  1.70it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.57it/s]
                   all        100        196      0.871      0.822      0.866      0.516

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    284/999      12.4G    0.01706   0.007459  0.0009699         68        640: 100% 10/10 [00:06<00:00,  1.55it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.54it/s]
                   all        100        196      0.827      0.822      0.851      0.512

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    285/999      12.4G    0.01681   0.007236   0.001669         66        640: 100% 10/10 [00:05<00:00,  1.69it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.54it/s]
                   all        100        196      0.859      0.822      0.867      0.503

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    286/999      12.4G      0.017   0.007661   0.001539         75        640: 100% 10/10 [00:06<00:00,  1.57it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.54it/s]
                   all        100        196      0.947      0.769       0.87      0.522

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    287/999      12.4G    0.01718   0.007489   0.001404         68        640: 100% 10/10 [00:05<00:00,  1.69it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.54it/s]
                   all        100        196      0.921      0.818      0.881      0.524

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    288/999      12.4G    0.01653   0.007318   0.001005         62        640: 100% 10/10 [00:06<00:00,  1.57it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.56it/s]
                   all        100        196      0.905      0.852      0.902      0.532

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    289/999      12.4G    0.01697   0.008511   0.001276         68        640: 100% 10/10 [00:05<00:00,  1.69it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.56it/s]
                   all        100        196      0.955      0.806      0.894      0.532

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    290/999      12.4G     0.0164   0.007877  0.0009936         92        640: 100% 10/10 [00:06<00:00,  1.56it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.55it/s]
                   all        100        196      0.938      0.812      0.899      0.537

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    291/999      12.4G    0.01756   0.007131  0.0009895         82        640: 100% 10/10 [00:05<00:00,  1.68it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.57it/s]
                   all        100        196      0.887      0.856      0.892      0.518

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    292/999      12.4G    0.01742   0.007367   0.001097         69        640: 100% 10/10 [00:06<00:00,  1.55it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.55it/s]
                   all        100        196      0.889      0.864      0.902      0.516

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    293/999      12.4G    0.01731   0.007165   0.001069         47        640: 100% 10/10 [00:05<00:00,  1.67it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.56it/s]
                   all        100        196      0.877      0.834      0.875      0.513

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    294/999      12.4G    0.01716   0.007549   0.001133         64        640: 100% 10/10 [00:06<00:00,  1.55it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.49it/s]
                   all        100        196      0.874      0.847      0.885       0.53

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    295/999      12.4G    0.01614   0.007524   0.000722         68        640: 100% 10/10 [00:05<00:00,  1.68it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.52it/s]
                   all        100        196      0.887      0.819      0.874      0.521

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    296/999      12.4G    0.01764   0.007291   0.001157         63        640: 100% 10/10 [00:06<00:00,  1.59it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.56it/s]
                   all        100        196      0.869      0.828      0.879      0.522

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    297/999      12.4G    0.01689   0.008237   0.001109         62        640: 100% 10/10 [00:05<00:00,  1.69it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.56it/s]
                   all        100        196      0.873      0.836      0.888      0.537

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    298/999      12.4G    0.01789   0.007301  0.0008347         65        640: 100% 10/10 [00:06<00:00,  1.58it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.57it/s]
                   all        100        196      0.909      0.802      0.869       0.52

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    299/999      12.4G    0.01513   0.007077  0.0009072         64        640: 100% 10/10 [00:05<00:00,  1.68it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.56it/s]
                   all        100        196      0.866      0.815       0.87      0.515

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    300/999      12.4G    0.01655   0.007587    0.00103         71        640: 100% 10/10 [00:06<00:00,  1.59it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.57it/s]
                   all        100        196      0.913      0.819      0.878      0.521

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    301/999      12.4G    0.01659   0.006348   0.001172         57        640: 100% 10/10 [00:05<00:00,  1.69it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.56it/s]
                   all        100        196      0.926      0.797       0.88      0.513

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    302/999      12.4G     0.0169   0.007095  0.0009448         65        640: 100% 10/10 [00:06<00:00,  1.53it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.54it/s]
                   all        100        196      0.875      0.834      0.878      0.504

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    303/999      12.4G    0.01647    0.00724  0.0009229         68        640: 100% 10/10 [00:05<00:00,  1.67it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.46it/s]
                   all        100        196      0.897       0.83      0.881      0.516

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    304/999      12.4G    0.01563   0.007447  0.0007962         79        640: 100% 10/10 [00:06<00:00,  1.59it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.55it/s]
                   all        100        196      0.892      0.833      0.877      0.521

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    305/999      12.4G    0.01567   0.007103   0.001199         61        640: 100% 10/10 [00:05<00:00,  1.68it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.36it/s]
                   all        100        196      0.832      0.821      0.862      0.499

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    306/999      12.4G    0.01604     0.0077    0.00114         73        640: 100% 10/10 [00:06<00:00,  1.59it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.55it/s]
                   all        100        196      0.834      0.813      0.858      0.495

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    307/999      12.4G    0.01572   0.007327    0.00134         69        640: 100% 10/10 [00:05<00:00,  1.68it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.36it/s]
                   all        100        196      0.856      0.827      0.867      0.496

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    308/999      12.4G    0.01647   0.007526   0.000791         61        640: 100% 10/10 [00:06<00:00,  1.63it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.54it/s]
                   all        100        196      0.852      0.837      0.862      0.506

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    309/999      12.4G    0.01566   0.007264   0.001014         99        640: 100% 10/10 [00:05<00:00,  1.68it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.37it/s]
                   all        100        196      0.837      0.814      0.846        0.5

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    310/999      12.4G    0.01646   0.006707  0.0009148         72        640: 100% 10/10 [00:06<00:00,  1.63it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.56it/s]
                   all        100        196       0.91      0.806      0.875      0.511

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    311/999      12.4G    0.01704   0.007455   0.001363         61        640: 100% 10/10 [00:06<00:00,  1.66it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.38it/s]
                   all        100        196      0.927      0.774      0.862      0.509

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    312/999      12.4G    0.01548   0.007221   0.001161         63        640: 100% 10/10 [00:06<00:00,  1.65it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.56it/s]
                   all        100        196      0.857      0.808      0.859      0.512

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    313/999      12.4G    0.01624   0.007353    0.00116         58        640: 100% 10/10 [00:06<00:00,  1.66it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.32it/s]
                   all        100        196      0.855      0.808      0.862       0.51

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    314/999      12.4G    0.01598   0.006753   0.001468         53        640: 100% 10/10 [00:05<00:00,  1.67it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.52it/s]
                   all        100        196      0.872      0.809      0.863      0.516

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    315/999      12.4G    0.01519   0.007092   0.001073         81        640: 100% 10/10 [00:06<00:00,  1.65it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.29it/s]
                   all        100        196      0.865      0.825      0.868      0.518

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    316/999      12.4G     0.0154   0.007031   0.001164         79        640: 100% 10/10 [00:05<00:00,  1.69it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.55it/s]
                   all        100        196      0.892      0.824      0.876      0.512

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    317/999      12.4G    0.01562   0.006812   0.001104         64        640: 100% 10/10 [00:06<00:00,  1.63it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.33it/s]
                   all        100        196       0.93      0.789      0.875      0.512

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    318/999      12.4G     0.0161   0.007212  0.0008151         72        640: 100% 10/10 [00:05<00:00,  1.70it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.56it/s]
                   all        100        196      0.937      0.788       0.88      0.519

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    319/999      12.4G    0.01502    0.00669   0.001024         73        640: 100% 10/10 [00:06<00:00,  1.59it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.35it/s]
                   all        100        196      0.925      0.822      0.882      0.525

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    320/999      12.4G    0.01606   0.007093   0.001102         59        640: 100% 10/10 [00:05<00:00,  1.70it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.55it/s]
                   all        100        196      0.924      0.806      0.887      0.534

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    321/999      12.4G    0.01584   0.007239   0.001175         69        640: 100% 10/10 [00:06<00:00,  1.62it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.37it/s]
                   all        100        196      0.918      0.827      0.889      0.537

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    322/999      12.4G    0.01508   0.006881   0.001169         85        640: 100% 10/10 [00:05<00:00,  1.69it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.59it/s]
                   all        100        196      0.879      0.858      0.891      0.533

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    323/999      12.4G    0.01577   0.006114  0.0008509         64        640: 100% 10/10 [00:06<00:00,  1.62it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.39it/s]
                   all        100        196      0.862      0.849       0.88      0.525

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    324/999      12.4G    0.01626    0.00733    0.00107         54        640: 100% 10/10 [00:05<00:00,  1.69it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.57it/s]
                   all        100        196      0.899      0.815       0.86      0.522

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    325/999      12.4G    0.01694   0.007495   0.001136         61        640: 100% 10/10 [00:06<00:00,  1.60it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.36it/s]
                   all        100        196      0.944      0.784      0.859      0.516

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    326/999      12.4G    0.01526   0.006741   0.001103         82        640: 100% 10/10 [00:05<00:00,  1.68it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.55it/s]
                   all        100        196      0.904      0.833      0.881      0.513

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    327/999      12.4G    0.01636   0.007268   0.001538         62        640: 100% 10/10 [00:06<00:00,  1.56it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.56it/s]
                   all        100        196      0.915      0.833      0.873      0.524

      Epoch    GPU_mem   box_loss   obj_loss   cls_loss  Instances       Size
    328/999      12.4G    0.01671    0.00705   0.001221         75        640: 100% 10/10 [00:05<00:00,  1.69it/s]
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 2/2 [00:01<00:00,  1.55it/s]
                   all        100        196      0.916      0.825      0.869      0.521
  ```
</details>

### Evidências do treinamento

Batch
![Batch](https://github.com/rutealvesdc/CESAR-School/blob/main/Redes-Neurais/assets/val_batch0_pred.jpg)

Loss
![Loss](https://github.com/rutealvesdc/CESAR-School/blob/main/Redes-Neurais/assets/W%26B%20Chart%2001_05_2023%2012%2004%2012.png)

Precision
![Precision](https://github.com/rutealvesdc/CESAR-School/blob/main/Redes-Neurais/assets/W%26B%20Chart%2001_05_2023%2012%2002%2004.png)

Confusion Matrix
![Confusion Matrix](https://github.com/rutealvesdc/CESAR-School/blob/main/Redes-Neurais/assets/confusion_matrix.png)

## Roboflow

Link para acessar o dataset no Roboflow: [helmet_etc_dataset](https://app.roboflow.com/rac3/helmet_etc_dataset/1)
