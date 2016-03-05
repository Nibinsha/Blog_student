from __future__ import unicode_literals

from django.db import models
from django.utils import timezone


class Post(models.Model):
  
    Name = models.CharField(max_length=200)
    Address = models.TextField()
    RollNo = models.IntegerField(default=0)
    Maths = models.IntegerField(default=0)
    Physics = models.IntegerField(default=0)
    Chemistry = models.IntegerField(default=0)
    created_date = models.DateTimeField(
            default=timezone.now)
    published_date = models.DateTimeField(
            blank=True, null=True)

    def publish(self):
        self.published_date = timezone.now()
        self.save()

    def __str__(self):
        return self.Name

# Create your models here.
