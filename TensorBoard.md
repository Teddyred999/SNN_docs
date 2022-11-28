### TensorBoard

> #### **from torch.utils import tensorboard**

1.  pip install tensorboard(manipulate in console)
   * tensorboard --logdir=runs

2.  Some part

   * tensorboard.SummaryWriter

     ```python
     from torch.utils import tensorboard
     writer = tensorboard.SummaryWriter('dir')  # set up writer log path
     
     # add imgs
     img_grid = torchvision.utils.mark_grid(a batch imgs)  # build a img grid
     writer.add_image(tag, img_grid)  # put tag and img_grid in writer[CHW]
     writer.add_images(tag, img_grid)  # put tag and img_grid in writer[NCHW]
     writer.close()  # flush writer
     """sys.exit() 提前终止"""
     
     # add model graph
     writer.add_graph(model, a batch imgs)
     
     # add loss/acc
     writer.add_scalar('training loss', loss, index)
     ```

     

